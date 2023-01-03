<template>
  <h2>Hello</h2>
  </template>
  
  <script>
  export default {
    data() {
      return {
        quiz: {
          fullName: "Sky Albert",
          email: "",
          desc: "",
          jobs: [],
        },
        error: {
          text: "",
          status: false,
        },
        success: {
          text: "",
          status: false,
        },
        jobOptions: [
          {
            id: 1,
            name: "Branding",
          },
          {
            id: 2,
            name: "Strategy",
          },
          {
            id: 3,
            name: "Motion Design",
          },
          {
            id: 4,
            name: "Development",
          },
          {
            id: 5,
            name: "Product Design",
          },
          {
            id: 6,
            name: "Marketing",
          },
          {
            id: 7,
            name: "Copywriting",
          },
          {
            id: 8,
            name: "Advisory",
          },
          {
            id: 9,
            name: "Compositing",
          },
        ],
      };
    },
    methods: {
      onSubmit() {
        console.log(this.quiz);
        if (this.quiz.fullName.length < 6 || this.quiz.fullName.length > 18) {
          this.error = {
            text: "Look failed! Full Name should be 6-18 characters.",
            status: true,
          };
        } else if (
          this.quiz.fullName.length > 5 &&
          this.quiz.fullName.length < 19
        ) {
          this.success = {
            text: "Look great!",
            status: true,
          };
        } else {
          this.error = {
            text: "",
            status: false,
          };
        }
      },
    },
  };
  </script>