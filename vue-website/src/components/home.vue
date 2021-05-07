<template>
  <div class="wrapper">
    <div id="about-me" class="page dark-bg">
      <div class="full-height large-width left center-vertically">
        <div id="title" class="bold title margin-left">Hi, I'm Axelle Jamous, a Software Developer</div>
        <button id="email-button" class="margin-left" @click="mailToMe()">Email me</button>
        <div class="icons">
          <a id="svg-github" href="https://github.com/axellejamous" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 256 250" version="1.1" preserveAspectRatio="xMidYMid">
              <g>
                <path d="M128.00106,0 C57.3172926,0 0,57.3066942 0,128.00106 C0,184.555281 36.6761997,232.535542 87.534937,249.460899 C93.9320223,250.645779 96.280588,246.684165 96.280588,243.303333 C96.280588,240.251045 96.1618878,230.167899 96.106777,219.472176 C60.4967585,227.215235 52.9826207,204.369712 52.9826207,204.369712 C47.1599584,189.574598 38.770408,185.640538 38.770408,185.640538 C27.1568785,177.696113 39.6458206,177.859325 39.6458206,177.859325 C52.4993419,178.762293 59.267365,191.04987 59.267365,191.04987 C70.6837675,210.618423 89.2115753,204.961093 96.5158685,201.690482 C97.6647155,193.417512 100.981959,187.77078 104.642583,184.574357 C76.211799,181.33766 46.324819,170.362144 46.324819,121.315702 C46.324819,107.340889 51.3250588,95.9223682 59.5132437,86.9583937 C58.1842268,83.7344152 53.8029229,70.715562 60.7532354,53.0843636 C60.7532354,53.0843636 71.5019501,49.6441813 95.9626412,66.2049595 C106.172967,63.368876 117.123047,61.9465949 128.00106,61.8978432 C138.879073,61.9465949 149.837632,63.368876 160.067033,66.2049595 C184.49805,49.6441813 195.231926,53.0843636 195.231926,53.0843636 C202.199197,70.715562 197.815773,83.7344152 196.486756,86.9583937 C204.694018,95.9223682 209.660343,107.340889 209.660343,121.315702 C209.660343,170.478725 179.716133,181.303747 151.213281,184.472614 C155.80443,188.444828 159.895342,196.234518 159.895342,208.176593 C159.895342,225.303317 159.746968,239.087361 159.746968,243.303333 C159.746968,246.709601 162.05102,250.70089 168.53925,249.443941 C219.370432,232.499507 256,184.536204 256,128.00106 C256,57.3066942 198.691187,0 128.00106,0 Z M47.9405593,182.340212 C47.6586465,182.976105 46.6581745,183.166873 45.7467277,182.730227 C44.8183235,182.312656 44.2968914,181.445722 44.5978808,180.80771 C44.8734344,180.152739 45.876026,179.97045 46.8023103,180.409216 C47.7328342,180.826786 48.2627451,181.702199 47.9405593,182.340212 Z M54.2367892,187.958254 C53.6263318,188.524199 52.4329723,188.261363 51.6232682,187.366874 C50.7860088,186.474504 50.6291553,185.281144 51.2480912,184.70672 C51.8776254,184.140775 53.0349512,184.405731 53.8743302,185.298101 C54.7115892,186.201069 54.8748019,187.38595 54.2367892,187.958254 Z M58.5562413,195.146347 C57.7719732,195.691096 56.4895886,195.180261 55.6968417,194.042013 C54.9125733,192.903764 54.9125733,191.538713 55.713799,190.991845 C56.5086651,190.444977 57.7719732,190.936735 58.5753181,192.066505 C59.3574669,193.22383 59.3574669,194.58888 58.5562413,195.146347 Z M65.8613592,203.471174 C65.1597571,204.244846 63.6654083,204.03712 62.5716717,202.981538 C61.4524999,201.94927 61.1409122,200.484596 61.8446341,199.710926 C62.5547146,198.935137 64.0575422,199.15346 65.1597571,200.200564 C66.2704506,201.230712 66.6095936,202.705984 65.8613592,203.471174 Z M75.3025151,206.281542 C74.9930474,207.284134 73.553809,207.739857 72.1039724,207.313809 C70.6562556,206.875043 69.7087748,205.700761 70.0012857,204.687571 C70.302275,203.678621 71.7478721,203.20382 73.2083069,203.659543 C74.6539041,204.09619 75.6035048,205.261994 75.3025151,206.281542 Z M86.046947,207.473627 C86.0829806,208.529209 84.8535871,209.404622 83.3316829,209.4237 C81.8013,209.457614 80.563428,208.603398 80.5464708,207.564772 C80.5464708,206.498591 81.7483088,205.631657 83.2786917,205.606221 C84.8005962,205.576546 86.046947,206.424403 86.046947,207.473627 Z M96.6021471,207.069023 C96.7844366,208.099171 95.7267341,209.156872 94.215428,209.438785 C92.7295577,209.710099 91.3539086,209.074206 91.1652603,208.052538 C90.9808515,206.996955 92.0576306,205.939253 93.5413813,205.66582 C95.054807,205.402984 96.4092596,206.021919 96.6021471,207.069023 Z" fill="#161614"/>
              </g>
            </svg>
          </a>
          <a id="svg-linkedin" href="https://www.linkedin.com/in/axelle-jamous/" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 72 72" version="1.1">
              <title>Linkedin</title>
              <defs/>
              <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                <g id="Social-Icons---Rounded-Black" transform="translate(-376.000000, -267.000000)">
                  <g id="Linkedin" transform="translate(376.000000, 267.000000)">
                    <path d="M8,72 L64,72 C68.418278,72 72,68.418278 72,64 L72,8 C72,3.581722 68.418278,-8.11624501e-16 64,0 L8,0 C3.581722,8.11624501e-16 -5.41083001e-16,3.581722 0,8 L0,64 C5.41083001e-16,68.418278 3.581722,72 8,72 Z" id="Rounded" fill="#000000"/>
                    <path id="svg-linkedin-innerpath" d="M62,62 L51.315625,62 L51.315625,43.8021149 C51.315625,38.8127542 49.4197917,36.0245323 45.4707031,36.0245323 C41.1746094,36.0245323 38.9300781,38.9261103 38.9300781,43.8021149 L38.9300781,62 L28.6333333,62 L28.6333333,27.3333333 L38.9300781,27.3333333 L38.9300781,32.0029283 C38.9300781,32.0029283 42.0260417,26.2742151 49.3825521,26.2742151 C56.7356771,26.2742151 62,30.7644705 62,40.051212 L62,62 Z M16.349349,22.7940133 C12.8420573,22.7940133 10,19.9296567 10,16.3970067 C10,12.8643566 12.8420573,10 16.349349,10 C19.8566406,10 22.6970052,12.8643566 22.6970052,16.3970067 C22.6970052,19.9296567 19.8566406,22.7940133 16.349349,22.7940133 Z M11.0325521,62 L21.769401,62 L21.769401,27.3333333 L11.0325521,27.3333333 L11.0325521,62 Z" fill="#FFFFFF"/>
                  </g>
                </g>
              </g>
            </svg>
          </a>
          <a id="svg-stackoverflow" href="https://stackoverflow.com/users/1780110/axelle?tab=profile" target="_blank">
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 38 48" version="1.1">
              <title>stackoverflow</title>
              <defs/>
              <g id="Page-1" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                <g id="Social-Icons---Isolated" transform="translate(-505.000000, -1175.000000)">
                  <g id="stackoverflow" transform="translate(505.000000, 1175.000000)">
                    <path d="M25.0860128,41.5922927 L5.97459514,41.6011499 L5.97294973,37.5538824 L25.0835447,37.5440929 L25.0860128,41.5922927 L25.0860128,41.5922927 Z M38,18.6708298 L34.7306912,0 L30.7087256,0.692025863 L33.9775643,19.3628557 L38,18.6708298 L38,18.6708298 Z M25.5455518,32.3547147 L6.51569942,30.616026 L6.14101644,34.6470941 L25.1712214,36.3841513 L25.5455518,32.3547147 L25.5455518,32.3547147 Z M26.8009984,27.0731519 L8.34598112,22.1539179 L7.28563299,26.0621508 L25.7419431,30.9819676 L26.8009984,27.0731519 L26.8009984,27.0731519 Z M29.2103463,22.4436411 L12.7494464,12.8164635 L10.6748215,16.3015328 L27.1365441,25.9292931 L29.2103463,22.4436411 L29.2103463,22.4436411 Z M33.2466504,19.6088756 L22.4792159,3.95170309 L19.106599,6.23184556 L29.8745036,21.8883189 L33.2466504,19.6088756 L33.2466504,19.6088756 Z" fill="#FF810F"/>
                    <polygon id="stackoverflow-icon-path" fill="#BEBCBC" points="28.3315807 28.2784283 28.3315807 44.8243495 3.2648427 44.8243495 3.2648427 28.2784283 0 28.2784283 0 48 31.5799693 48 31.5799693 28.2784283"/>
                  </g>
                </g>
              </g>
            </svg>
          </a>
        </div>
      </div>
      <div id="codejar-wrapper" class="full-height small-width right center-vertically">
        <codejar />
      </div>
    </div>
    <div id="background" class="page-half">
      <div class="full-height larger-width left center-vertically">
        <div class="info">
          <div class="medium-title">― My background</div>
          <div>
            I thoroughly enjoy the development process from beginning to end, keeping the user's experience front and center. I'm extremely motivated to constantly develop my skills to grow both on a technical and professional level.
            I enjoy responsibility and strive to always deliver the best approach to what the client wants and needs.
          </div>
        </div>
      </div>
      <div class="full-height smaller-width right center-vertically">
        <div class="info">
          <div class="medium-title">― Skills</div>
          <ul>
            <li>Problem solving</li>
            <li>Self motivation</li>
            <li>Decisiveness</li>
            <li>Adaptability</li>
            <li>Teamwork</li>
          </ul>
        </div>
      </div>
    </div>
    <div id="cv" class="dark-bg">
      <div class="full-height center-vertically">
        <table class="cv-table">
          <tr>
            <td class="medium-title smaller-width td-head">― Work experience</td>
            <td class="larger-width">
              <div class="td-row-wrapper">
                <div class="td-title">Software Developer Consultant</div>
                <div class="td-subtitle">Soluz.io  / Sept 2020 - Present</div>
                <div>I have been working on the integration of modern ERP systems into the Soluz.io platform as well as end-to-end, fully custom, software applications built on top of the Soluz.io platform.</div>
              </div>
              <div class="td-row-wrapper">
                <div class="td-title">Software Developer / Business Solution Expert</div>
                <div class="td-subtitle">Arco Information  / May 2019 - Present</div>
                <div>I’ve been central to delivering two IoT MvP's as well as an end-to-end web application in the online marketplace space, both built on top of Arco Information's existing software platform.</div>
              </div>
              <div class="td-row-wrapper">
                <div class="td-title">Unity, Hardware & Full-Stack Developer</div>
                <div class="td-subtitle">Soulmade  / Dec 2018 - April 2019</div>
                <div>While at Soulmade, I helped establish a scrum/agile methodology workflow as well as mentored interns in the hardware development space. I was responsible for backend development in Unity as well as full stack development for web and mobile applications.</div>
              </div>
              <div class="td-row-wrapper">
                <div class="td-title">IoT Development intern</div>
                <div class="td-subtitle">BASF  / Sept 2018 - Feb 2019</div>
                <div>I very lucky to work with an experienced IoT developer and Proximus to help develop a MvP for a large scale project within the BASF 4.0 integration.</div>
              </div>
            </td>
          </tr>
          <tr>
            <td class="medium-title smaller-width td-head">― Education</td>
            <td class="larger-width">
              <div class="td-row-wrapper">
                <div class="td-title">AP University College</div>
                <div class="td-subtitle">Bachelor of Applied Science, Electronics-ICT  / 2017 - 2019</div>
              </div>
            </td>
          </tr>
        </table>
        <div>
          <div id="cv-download-wrapper">
            <lord-icon
                src="https://cdn.lordicon.com//nocovwne.json"
                trigger="hover"
                colors="primary:#121331,secondary:#08a88a"
                id="lordicon">
            </lord-icon>
            <a :href="`${publicPath}cv.pdf`" download="cv_AxelleJamous.pdf" target="_blank" class="download">Download full CV</a>
            <div class="clear"></div>
          </div>
        </div>
      </div>
    </div>
    <div id="contact" class="page-half light-bg">
      <div class="full-height small-width left center-vertically">
        <div class="big-title">Let's get in touch.</div>
      </div>
      <div id="contact-details-wrapper" class="full-height large-width right center-vertically-and-horizontally">
        <div class="contact-wrapper">
          <div class="medium-title">― Socials</div>
          <ul>
            <li><a href="https://www.linkedin.com/in/axelle-jamous/" target="_blank">LinkedIn</a></li>
            <li><a href="https://github.com/axellejamous" target="_blank">GitHub</a></li>
            <li><a href="https://stackoverflow.com/users/1780110/axelle?tab=profile" target="_blank">Stackoverflow</a></li>
          </ul>
        </div>
        <div class="contact-wrapper">
          <div class="medium-title">― Contact details</div>
          <ul>
            <li><a href="javascript:void(0);" @click="mailToMe()">Email</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="clear"></div>
  </div>
</template>

<script>
import codejar from "@/components/codejar.vue";

export default {
  components: { codejar },
  name: 'home',
  data () {
    return {
      publicPath: process.env.BASE_URL
    }
  },
  methods: {
    mailToMe: function () {
      location.href = "mailto:axellejamous@hotmail.com?subject=Found your website";
    }
  }
}
</script>

<style>
#about-me{
  position: relative;
}
#about-me #title{
  text-align: left;
}
#about-me #email-button{
  padding: 20px;
  border: unset;
  border-radius: 5px;
  background-color:#CBF1E4;
  width: 150px;
}
#background{
  background-color: #fff;
}
#svg-linkedin, #svg-stackoverflow{
  margin-left: 30px;
}
#svg-linkedin-innerpath{
  fill: #fff;
}
#svg-stackoverflow polygon{
  fill: rgb(44, 62, 80);
}
#cv-download-wrapper{
  margin-left: 30px;
  margin-bottom: 20px;
  display: flex;
  align-items: center;
}
#lordicon{
  width:50px;
  height:50px;
  float: left;
}
#lordicon:hover{
  cursor: pointer;
}

.icons{
  position: absolute;
  bottom: 100px;
  left: 30px;
}
.wrapper{
  width: 100%;
}
.page{
  height: 100vh;
}
.page-half{
  height: 50vh;
}
.dark-bg{
  background: #F5F7FA;
}
.light-bg{
  background: #cbf1e4;
}
.full-height{
  height: 100%;
}
.full-width{
  width: 100%;
}
.half-width{
  width: 50%;
}
.large-width{
  width: 60%;
}
.small-width{
  width: 40%;
}
.larger-width{
  width: 65%;
}
.smaller-width{
  width: 35%;
}
.left{
  float: left;
}
.right{
  float: right;
}
.clear{
  clear: both;
}
.center-vertically, .center-vertically-and-horizontally{
  display: flex;
}
.center-vertically{
  justify-content: center;
  flex-direction: column;
}
.center-vertically-and-horizontally{
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.title{
  font-size: 64px;
}
.medium-title{
  color: rgb(123, 136, 168);
  text-transform: uppercase;
  font-weight: bold;
  letter-spacing: 1px;
  margin-bottom: 20px;
}
.big-title{
  font-size: 50px;
  font-weight: bold;
}
.info{
  margin: 0 auto;
  width: 80%;
  text-align: left;
}
.light{
  font-weight: 300;
}
.bold{
  font-weight: 700;
}
.margin-left{
  margin-left: 30px;
}
.svg-img{
  height: 50px;
}
.td-head{
  padding-left: 80px;
  vertical-align: top;
}
.td-title{
  font-weight: bold;
  font-size: 22px;
  margin-bottom: 15px;
}
.td-subtitle{
  margin-bottom: 20px;
  font-size: 17px;
}
.td-row-wrapper{
  margin-bottom: 40px;
}
.download{
  font-size: 17px;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: bold;
  float: left;
}
.cv-table{
  margin-top: 100px;
  margin-bottom: 100px;
}
.cv-table > tr > td{
  text-align: left;
}
.cv-table > td {
  padding-bottom: 100px;
}
.cv-table > tr:last-child > td{
  padding-bottom: unset;
}
.contact-wrapper{
  text-align: left;
  height: 110px;
}
#contact-details-wrapper > div:first-child{
  margin-right: 100px;
}

@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  #codejar-wrapper{
    height: 40%;
  }

  .icons{
    bottom: 10px;
  }
  .cv-table{
    margin-top: 10px;
  }
  .cv-table>tr>td{
    padding-left: 20px;
    float: left;
  }
  .contact-table>tr>td, .contact-table>tr>th{
    width: 100%;
    float: left;
  }
  .contact-table > tr > td:first-child, .contact-table > tr > th:first-child {
    padding-right: unset;
  }
  .page-half{
    height: 100vh;
  }
  .title{
    font-size: 40px;
  }
  .half-width, .large-width, .small-width, .larger-width, .smaller-width{
    width: 100%;
  }
  .full-height{
    height: 50%;
  }
  .td-head {
    padding-left: 20px;
  }
  .download{
    padding-left: 20px;
  }
  #contact-details-wrapper > div:first-child {
    margin-right: unset;
  }
  .contact-wrapper {
    margin-left: 30px;
    margin-bottom: 50px;
  }
}
@media only screen and (max-width: 768px) and (orientation: portrait){
  .page-half{
    height: 75vh;
  }
  .center-vertically-and-horizontally{
    flex-direction: column;
    align-items: flex-start;
  }
  .contact-wrapper {
    height: unset;
  }
  .info{
    padding-top: 40px;
  }
  #cv-download-wrapper {
    margin-left: unset;
  }
}
@media only screen and (max-width: 768px) and (orientation: landscape){
  .page {
    height: 150vh;
  }
  .icons {
    bottom: -175px;
  }
}
</style>
