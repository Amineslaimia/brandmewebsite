<template>
  <div>
    <div id="surveyContainer">
      <div id="surveyContainer"><survey :survey="survey"></survey></div>
    </div>
  </div>
</template>
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.1.10/vue.min.js"></script>
<script src="https://unpkg.com/survey-vue"></script>
<script>
import * as Survey from "survey-vue";

import "bootstrap/dist/css/bootstrap.css";
var surveyJSON = {
  title: "Tell us, what technologies do you use?",
  pages: [
    {
      name: "page1",
      questions: [
        {
          type: "radiogroup",
          choices: ["Yes", "No"],
          isRequired: true,
          name: "frameworkUsing",
          title: "Do you use any front-end framework like Bootstrap?"
        },
        {
          type: "checkbox",
          choices: ["Bootstrap", "Foundation"],
          hasOther: true,
          isRequired: true,
          name: "framework",
          title: "What front-end framework do you use?",
          visibleIf: "{frameworkUsing} = 'Yes'"
        }
      ]
    },
    {
      name: "page2",
      questions: [
        {
          type: "radiogroup",
          choices: ["Yes", "No"],
          isRequired: true,
          name: "mvvmUsing",
          title: "Do you use any MVVM framework?"
        },
        {
          type: "checkbox",
          choices: ["AngularJS", "KnockoutJS", "React"],
          hasOther: true,
          isRequired: true,
          name: "mvvm",
          title: "What MVVM framework do you use?",
          visibleIf: "{mvvmUsing} = 'Yes'"
        }
      ]
    },
    {
      name: "page3",
      questions: [
        {
          type: "comment",
          name: "about",
          title:
            "Please tell us about your main requirements for Survey library"
        }
      ]
    }
  ]
};
var survey = new Survey.Model(surveyJSON);
export default {
  components: {
    survey
  },
  data() {
    return {
      data: { survey: survey }
    };
  }
};
</script>
