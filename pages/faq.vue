<template>
  <v-main>
    <v-container class="faqHead">
      <v-card>
        <v-card-text>
          <h1>Frequently Asked Questions</h1>
          <h4>More Frequent Than We Would Care to Admit</h4>
        </v-card-text>
      </v-card>
      <v-col>
        <h2>
          Where can I submit a ticket for a student?
        </h2>
        <h4> You can fill out a form <a href="https://docs.google.com/forms/d/e/1FAIpQLSdxqjaC_2f9lr5pZ7Y6XMoujUsPdKvW6ACuQAYn0cfCZpo61Q/viewform?usp=share_link">here</a></h4>
        <h2>How do I Submit a Ticket/Talk with MHIS</h2>
        <h4>
          You can email
          <a href="mailto:helpdesk@hartfordschools.org"> Helpdesk </a> , Call
          860-757-9411, or if You have an Account, you can submit a Ticket
          <a href="http://servicedesk.hartford.gov:8443" target="_blank"> here </a>
        </h4>
        <h2>My Student Needs a Loaner</h2>
        <h4>
          We are doing centralized loaners. You can have students get a loaner from Webster on the 3rd floor, or Silva on the 2nd floor.
        </h4>
        <h2>I suspect an email as Phishing/Someone Emailed me Trying to Extort Me </h2>
        <h4>
          Any email claiming to know information about you, asking for money, threatening you, or otherwise suspucious should be ignored
          and forwarded to <a href="mailto:suspiciousemails@hartfordschools.org"> suspiciousemails@hartfordschools.org </a>. 
          If you are concerned, you can also come see me or forward me the email.
        </h4> 

        <h2>When will my be Ticket Done?</h2>
        <h4>
          Well, we're probably pretty busy with our day jobs. You can see our
          workqueue <v-btn to="/ticketqueue"> here </v-btn> and see where you
          are in the priority list.
        </h4>

        <h2>I Need Tech Help, How do I Get it?</h2>
        <h4>
          You can submit a ticket <v-btn to="/newticket"> here </v-btn> and
          we'll come and help out when we have time
        </h4>

        <h2>Can I get a New Projector?</h2>
        <h4>
          Sadly we do not have any more new projectors to give out. We do have
          some TVs and carts for them if you'd want. Submit a ticket and we'll
          see what we can do.
        </h4>

        <h2>One of my Classroom Loaners is missing... Help?</h2>
        <h4>
          Send Dobbs an
          <a href="mailto:dobbb001@hartfordschools.org"> email </a> with which
          of your two loaners is missing and I'll try and find it
        </h4>

        <h2>A Student Says They Have a Broken Something or Other</h2>
        <h4>Send them down to 146 during 5th period and we'll sort it out</h4>

        <h2>Do you fix stuff other than school issued devices?</h2>
        <h4>
          Yes! We'll fix anything we can. Glasses, Phones, Playstations, Hats.
          Anything that is broken we will try and fix.
        </h4>

        <h2>Why did you make this website?</h2>
        <h4>We're nerds.</h4>
      </v-col>
    </v-container>
  </v-main>
</template>