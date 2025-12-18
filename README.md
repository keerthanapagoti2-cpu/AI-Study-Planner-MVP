<!DOCTYPE html>
<html>
<head>
    <title>AI Study Planner MVP</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; margin-top: 50px; }
        input, button { padding: 10px; margin: 5px; font-size: 16px; }
        #plan { margin-top: 30px; font-size: 18px; color: #333; }
    </style>
</head>
<body>
    <h1>AI Study Planner - MVP</h1>
    <p>Enter your subjects and available time:</p>
    <input type="text" placeholder="Subjects (Math, C, etc.)" id="subjects"><br>
    <input type="text" placeholder="Available time (hours)" id="time"><br>
    <button onclick="generatePlan()">Generate Plan</button>
    <div id="plan"></div>

    <script>
        function generatePlan() {
            var subjects = document.getElementById("subjects").value;
            var time = document.getElementById("time").value;
            var plan = "Sample Plan: Study " + subjects + " for " + time + " hours with breaks in between.";
            document.getElementById("plan").innerText = plan;
        }
    </script>
</body>
</html>
