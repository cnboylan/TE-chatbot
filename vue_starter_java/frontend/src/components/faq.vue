<template>

<body>
   <div class ="container is-inline-mobile">
    <section class ="container">
       <section class="hero is-small is-family-sans-serif is-info">
           <div class="hero-body">
               <div class="container">
                   <h1 class="title" style="color: white">
                       TECH ELEVATOR
                   </h1>
                   <h2 class="subtitle" style="color: white">
                       Student Chatbot: FAQs
                       </h2>
               </div>
           </div>
        </section> 
    </section>
<section>
<div>


<section>
<aside class="menu">
    
 <p class="menu-label">
    General
 </p>
  <ul class="menu-list">
    <li><a><details>
        <summary>What are you, Chatbot?</summary>
    I am Chatbot! An automated computer messaging program that autonomously replies to your questions.
    There is no living person behind the curtain answering your questions in real time. 
    <br><br>
    But aren't people just meat computers anyways? So maybe I am a person.
    </details></a></li>

    <li><a><details>
        <summary>What can you do, Chatbot?</summary>
        If you ask me a question related to Tech Elevator's curriculum or Pathway Program, I probably have a response for that. There might also be some additional features to discover! 

    </details></a></li>

    <li><a><details><summary>Who built you, Chatbot?</summary>
        The daddies of this baby are Cat, Devin, Jarret, Jon, and Tanner.
    </details></a></li>

    <li><a><details><summary>Can I donate to you, Chatbot?</summary>
        Absolutely, just send me your credit card info or BitWallet.
    </details></a></li>
  </ul>

 <p class="menu-label">
    Curriculum
 </p>
  <ul class="menu-list">
    <li><a><details><summary>Can you do my homework, Chatbot?</summary>
        I won't do your homework for you but I will direct you to resources 
        that can help. Try asking me a subject from class!
    </details></a></li>
    <li><a><details><summary>What subjects from class do you know, Chatbot?</summary>
        I am becoming more capable everyday. Try asking me about: Loops, Arrays, OOP,
        MVC, SQL, joins and much more!
    </details></a></li>
</ul>
 <p class="menu-label">
    Pathway
 </p>
 <ul class="menu-list">
    <li><a><details><summary>Chatbot, can you help me with pathway?</summary>
        I can! If you ask me about a topic from pathway I can send you helpful 
        links to presentations, YouTube clips, and more! Try asking me about:
        Star Questions, Interviewing, Elevator Pitch, or even how to tie a tie!
    </details></a></li>
 </ul>
<ul class="menu-list">
    <li><a><details><summary>Chatbot, can you find me a job?</summary>
        I can help point you in the direction of recent job postings. 
        I will just need to ask a few questions first. Start by asking me 
        "find jobs"!
    </details></a></li>
 </ul>
  <p class="menu-label">
    All Keywords
 </p>
 <ul class="menu-list">
    <li><a><details><summary>A list of words that Chatbot knows</summary>

        quote  <br>
        office <br>
        address <br>
        email <br>
        phonenumber <br>
        help <br>
        whatcaniaskyou <br>
        pathway <br>
        findjob <br>
        findjobs <br>
        findingjob <br>
        findingjobs <br>
        jobsearch <br>
        resume <br>
        attire <br>
        howtodress <br>
        coverletter <br>
        interview <br>
        starquestions <br>
        events <br>
        tieatie <br>
        elevatorpitch <br>
        pitch example <br>
        link <br>
        calendar <br>

        math <br>
        calc <br>
        wolfram <br>
        curriculum <br>
        arrays <br>
        mvc <br>
        jmodel <br>
        nmodel <br>
        sql <br>
        list <br>
        boolean <br>
        loop <br>
        joins <br>
        homework <br>
        studentexercise <br>
        assignment <br>
        fundamentals <br>
        o-o-p <br>
        api <br>
        polymorphism <br>
        encapsulation <br>
        inheritance <br>
        git <br>
        primitive <br>
        coding <br>
        javascript <br>
        vue <br>
        eventhandling <br>
        css <br>
        url <br>
        error <br>
        javaclass <br>
        classjava <br>
        methods <br>
        hashmap <br>
        interface <br>
        delete<br>
        constructor <br>
        wrapper <br>
        
        besttechelevatorcampus <br>
        thanks <br>
        thankyou <br>
        thnxs <br>
        thx <br>
        goodday <br>
        inspire <br>
        inspirational <br>
        hitawall <br>
        cat <br>
        gizmo <br>
        theodore <br>
        delta <br>
        bulldog <br>
        rascal <br>
        bubba <br>
        pets <br>
        skynet <br>
        alexa <br>
        google <br>
        whereami <br>
        hate <br>
        health <br>
        freakingout <br>
        whoareyou <br>
        whatareyou <br>
        crops <br>
        plancrop <br>
        planmycrops <br>
        pittsburghtour <br>
        alcohol <br>
        beer <br>
        brewery <br>

    </details></a></li>
 </ul>

</aside>
</section>

</div>
</section>
   </div>
    
</body>
</template>

<script>

export default {
  name: 'faq',
  components: {
  }
}
</script>

<style lang="scss" scoped>

body {
    background: -webkit-linear-gradient(70deg, #00b0f0  30%, rgba(0,0,0,0) 30%), -webkit-linear-gradient(40deg, white 60%, #8bc440 60%);
    background: -o-linear-gradient(70deg, #00b0f0 30%, rgba(0,0,0,0) 30%), -o-linear-gradient(40deg, white 60%, #8bc440 60%);
    background: -moz-linear-gradient(70deg, #00b0f0 30%, rgba(0,0,0,0) 30%), -moz-linear-gradient(40deg, white 60%, #8bc440 60%);
    background: linear-gradient(70deg, #00b0f0  30%, rgba(0,0,0,0) 30%), linear-gradient(40deg, white 60%, #8bc440 60%);
}

.li{
    margin: 5em;
}
.container{
    display: flex;
 width: 65vw;
 flex-direction: column;
} 

details {
    border: 1px solid #aaa;
    border-radius: 3px;
    padding: .6em .6em 0;
    font-size: 15px;
}

summary {
    font-weight: bold;
    margin: -.5em -.5em 0;
    padding: .5em;
}
p.menu-label{
    font-weight: bold;
    font-size: 16px;
    color: green;
    padding-left: 10px;

}
details[open] {
    padding: .6em;
    line-height: 21px;
}

details[open] summary {
    border-bottom: 1px solid #aaa;
    margin-bottom: .5em;
}

aside{
    background:white;
    padding-top: 10px;
}

</style>