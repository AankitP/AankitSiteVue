<template>
  <div class="holder">
    <div class="aboutMe">
      <p class="helloWorld">
        Hello World, My Name is 
      </p>
      <h1 class="myName">
        Aankit Pokhrel
      </h1>
      <div class="paragraph">
        <p>
          I am A Cyber Engineering Major at Louisiana Tech university<br/>
          I am currently a senior workign on my capstone, and am Projected to graduate in May
          <br/><br/>
          Before I set my mind on breaking into the tech field my plan was
          to go to medical school and become a doctor but
          the medical class that I took my sophomore year of highschool had other
          plans, I didn't find anything in that class interesting, I had taken a
          computer science class my freshman year, and I liked it alot. Throughout
          Highschool, I took Computer Science 1-3, AP computer science, Videogame
          design, a Cisco Networking class, and computer programming
          (in total 7 computer science related classes).
          <br/><br/>
          At Louisiana Tech I have taken classes such as Data Structures, Systems Programming,
          Intro to Microprocessors, Computer Network Security, Applied Cryptography, and many more.
          All of these classes have allowed me to grow my critical skill set, and I am ready to use
          the skills that I have accumulated in a professional work environment.
          <br/><br/>
          I have experience in many languages, but the language that I am most comfortable with is
          Python. Other languages that I have used include Java, C, C++, and JS. I am able to pickup languages
          relatively quickly. I am currently learning Web development with the REACT framework along with VUE and MUI
        </p>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: "AboutMe",
};
</script>


<style scoped>
.helloWorld{
  align-content: left;
  justify-content: left;
  text-align: left;
  color:aquamarine;
}
.myName{
  align-content: left;
  justify-content: left;
  text-align: left;
  color: #10c55c;
  font-size: 500%;
}
.holder{
  margin: 4rem;
  margin-right: 4rem;
  margin-left: 4rem;
  min-height: 80vh;
  height: auto;
  display: flex;
  align-items: center;
  background-color: #08355a;
  border-radius: 1rem;
}
.aboutMe {
  color: #ffffff;
  align-content: center;
  justify-content: center;
  text-align: center;
  margin: 3rem;
}
.paragraph{
  margin: 5rem;
  width: 65vw;
  height: 20rem;
}
</style>