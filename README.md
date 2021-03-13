# Eye-tracking
<html>
  <title>ABCDE</title>
  <script src="https://webgazer.cs.brown.edu/webgazer.js?" type="text/javascript"></script>
  <script type="text/javascript">
    window.onload = function() {
      webgazer.setGazeListener(function(data, elapsedTime) {
        if (data == null) {
          return;
        }
        var xprediction = data.x; //these x coordinates are relative to the viewport
        var yprediction = data.y; //these y coordinates are relative to the viewport
        console.log(elapsedTime); //elapsed time is based on time since begin was called
      }).begin();
    };
  </script>
</html>
