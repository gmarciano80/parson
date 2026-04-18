<div id="test-sortableTrash" class="sortable-code"></div> 
<div id="test-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="test-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="test-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Hello World&quot;)\n" +
    "print Hello\n" +
    "#distractor\n" +
    "Prinmt(Hello)#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "test-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "test-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#test-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#test-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
<div id="test-sortableTrash" class="sortable-code"></div> 
<div id="test-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="test-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="test-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 

<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Ciao&quot;)\n" +
    "print(&quot;Come ti chiami?)\n" +
    "print(&quot;ho fame&quot;)#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "test-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "test-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#test-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#test-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

