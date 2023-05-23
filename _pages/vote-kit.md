---
layout: default
permalink: /vote-kit

author: eclub
logo:
  url: logo/rotaract-alpha.png
  position: center

pretitle: How to start a vote
title: Vote Kit
description: Message templates for Internal group chat

links-side: true

links-home: false

links-gallery:
  - left:
      name: E-ROTARACT BEYOND FRONTIERS<br>We are Rotaract – Join us today!
      image: logo/rotaract-pink.png
      url: /
      newtab: false
    right:
      name: FOLLOW US<br>Get to know us on Instagram!
      image: instagram-logo.jpg
      url: /instagram
      newtab: true

links-footer:
  - name: rotaract_eclub
    icon: fab fa-instagram
    url: /instagram
    newtab: true

show-notif: false

---

# Vote Information

- Vote number (this year): <input id="vote_nr" value=""/>
- Curent number of Members: <input id="members" value=""/>
- Decision: <input id="decision" value=""/>

# Simple Vote

<pre style="font-size: 15px;" id="simplevote">
📌 Vote <span id="vote_nr_text">00</span>x<script>document.write(new Date().getFullYear());</script>
🗳 *Decision: <span id="decision_text">..</span>.*
✅ To vote “Yes”, no action is needed, since the absence of vote is a “Yes”.
❎ To vote “No”, go to e-rotaract.com/vote, write what you disagree with, and give ideas. For disapproval, “No” votes must be ≥40% (<span id="members_no_text">0</span> Members).
⏰ This vote ends in 10 days: <script>
var d = new Date(new Date().getTime()+867_600_000).toISOString().split(".")[0].substring(0, 16).replace('T', ', at ');
document.write(d);
</script> UTC.
</pre>

{% include gallery-btn
  large=true
  items='[
    { name: "Copy Simple Vote", icon: "fas fa-vote-yea fa-lg", url: "javascript:navigator.clipboard.writeText($(\'#simplevote\').clone().children().remove().end().text())" }
  ]'
%}

# Urgent Vote

- Justification (if it is Urgent): <input id="justification" value=""/>

<pre style="font-size: 15px;" id="urgentvote">
📌 Vote <span id="vote_nr_text">00</span>x<script>document.write(new Date().getFullYear());</script>
🗳 *Urgent Decision: <span id="decision2_text">..</span>.*
⚠️ Justification for Urgency: <span id="justification_text">..</span>.
✅ To vote “Yes”, write it at e-rotaract.com/vote. For approval, “Yes” votes must be >60% (<span id="members_yes_text">0</span> Members). The absence of a vote is considered a “Yes”.
❎ To vote “No”, go to e-rotaract.com/vote, write what you disagree with, and give ideas. For disapproval, “No” votes must be ≥40% (<span id="members_no2_text">0</span> Members).
⏰ This vote ends in 48 hours: <script>
var d = new Date(new Date().getTime()+176_400_000).toISOString().split(".")[0].substring(0, 16).replace('T', ', at ');
document.write(d);
</script> UTC.
</pre>

{% include gallery-btn
  large=true
  items='[
    { name: "Copy Urgent Vote", icon: "fas fa-exclamation-triangle fa-lg", url: "javascript:navigator.clipboard.writeText($(\'#urgentvote\').clone().children().remove().end().text())" }
  ]'
%}

<script>
$("#vote_nr").on("keyup change", function(e) { $("#vote_nr_text").html(String($("#vote_nr").val()*1).padStart(2, '0')); });
$("#decision").on("keyup change", function(e) { $("#decision_text").html($("#decision").val());
  $("#decision2_text").html($("#decision").val());
});
$("#members").on("keyup change", function(e) { $("#members_no_text").html( Math.ceil($("#members").val()*0.4) );
  $("#members_no2_text").html( Math.ceil($("#members").val()*0.4) );
  $("#members_yes_text").html( Math.floor($("#members").val()*0.6)+1 );
});
$("#justification").on("keyup change", function(e) { $("#justification_text").html($("#justification").val()); });
</script>