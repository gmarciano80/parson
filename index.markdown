<div id="es1-sortableTrash" class="sortable-code"></div> 
<div id="es1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="es1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="es1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "if(true)
\n" +
    "    print(&quot;Qui sono nell&#039;if&quot;)
\n" +
    "    print(&quot;anche qui sono nell&#039;if&quot;)
\n" +
    "print(&quot;qui sono fuori dall&#039;if&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "es1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#es1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#es1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
<div id="es1-sortableTrash" class="sortable-code"></div> 
<div id="es1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="es1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="es1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "while(true)
\n" +
    "    print(&quot;Qui sono nel while&quot;)
\n" +
    "    print(&quot;anche qui sono nel while&quot;)
\n" +
    "print(&quot;qui sono fuori dal while&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "es1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#es1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#es1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
</script>
