<template>
    <div class="window">
        <div class="window-header">
            <div class="action-buttons"></div>
            <div class="controls">
                <div>language: <a class="switch-language" href="">js</a></div>
            </div>
        </div>
        <div class="window-body">
            <div id="codejar" class="editor language-js" data-gramm="false"></div>
        </div>
    </div>
</template>

<script>
import { CodeJar } from 'codejar';
import hljs from 'highlight.js';

export default {
  name: 'codejar',
  mounted: function() {
    const editor = document.getElementById("codejar");
    const highlight = (editor) => {
        hljs.highlightElement(editor);
    };
    var jar = CodeJar(document.getElementById('codejar'), highlight);

    let currentStyle = 6;
    const styles = [
      "dracula",
      "github",
      "solarized-dark",
      "solarized-light",
      "railscasts",
      "monokai-sublime",
      "mono-blue",
      "tomorrow",
      "color-brewer",
      "zenburn",
      "agate",
      "androidstudio",
      "atom-one-light",
      "rainbow",
      "vs",
      "atom-one-dark"
    ].map((name) => {
      const link = document.createElement("link");
      link.href = `https://cdnjs.cloudflare.com/ajax/libs/highlight.js/9.18.1/styles/${name}.min.css`;
      link.rel = "stylesheet";
      link.disabled = "true";
      document.head.appendChild(link);
      return link;
    });
    styles[currentStyle].removeAttribute("disabled");
    
    let currentLanguage = 0;
    const languages = [
    function () {
        editor.className = "editor language-js";
        jar.updateCode(`import {CodeJar} from '@medv/codejar';
import Prism from 'prismjs';

const editor = document.querySelector('#editor');
const jar = new CodeJar(editor, Prism.highlightElement, {tab: '\\t'});

// Update code
jar.updateCode('let foo = bar');

// Get code
let code = jar.toString();

// Listen to updates
jar.onUpdate(code => {
  console.log(code);
});
        `);
        jar.updateOptions({ tab: "  " });
    },
    function () {
        editor.className = "editor language-ts";
        jar.updateCode(`interface Person {
    firstName: string;
    lastName: string;
}

function greeter(person: Person) {
    return "Hello, " + person.firstName + " " + person.lastName;
}

let user = {
    firstName: "Jane",
    lastName: "User"
};

document.body.textContent = greeter(user);`);
        jar.updateOptions({ tab: "    " });
    },
    function () {
        editor.className = "editor language-html";
        jar.updateCode(`<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8">

  <title>CodeJar</title>

  <meta name="author" content="Anton Medvedev">
  <meta name="description" content="Micro Code Editor">
</head>
<body>
  <h1>CodeJar — Micro Code Editor</h1>
</body>
</html>`);
        jar.updateOptions({ tab: "  " });
    }
    ];

    languages[currentLanguage]();

    const switchLanguageButton = document.querySelector(".switch-language");
    switchLanguageButton.addEventListener("click", (event) => {
        event.preventDefault();
        currentLanguage = (currentLanguage + 1) % languages.length;
        languages[currentLanguage]();
        const [, name] = editor.className.match(/language-(\w+)/);
        switchLanguageButton.textContent = name;
    });
    }
}
</script>

<style scoped>
#codejar{
  font-family: 'Lato';
  text-align: left;
}

.window {
  width: 90%;
  margin: 0 auto;
  border-radius: 6px;
  box-shadow: 0 8px 12px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  overflow-y: auto;
  margin-bottom: 20px;
}
.window .window-header {
  height: 25px;
  background: Gainsboro;
  position: relative;
}
.window .window-header .action-buttons {
  position: absolute;
  top: 50%;
  left: 10px;
  margin-top: -5px;
  width: 10px;
  height: 10px;
  background: Crimson;
  border-radius: 50%;
  box-shadow: 15px 0 0 Orange, 30px 0 0 LimeGreen;
}
.editor {
  border-bottom-left-radius: 6px;
  border-bottom-right-radius: 6px;
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.14), 0 1px 5px 0 rgba(0, 0, 0, 0.12),
    0 3px 1px -2px rgba(0, 0, 0, 0.2);
  font-size: 14px;
  font-weight: 400;
  min-height: 340px;
  letter-spacing: normal;
  line-height: 20px;
  padding: 10px;
  resize: none !important;
  tab-size: 4;
}
.editor.hljs {
  padding: 10px;
}
.controls {
  font-size: 14px;
  position: absolute;
  top: 50%;
  right: 10px;
  margin-top: -10px;
  display: flex;
}
.controls > div:first-child > a {
  display: inline-block;
  width: 40px;
}
.switch-language{
    text-align: left;
}
</style>