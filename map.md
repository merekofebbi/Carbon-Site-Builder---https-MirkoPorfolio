---
layout: page
title: Map
permalink: /map
---
<!-- <iframe
  width="600"
  height="450"
  style="border:0"
  loading="lazy"
  allowfullscreen
  referrerpolicy="no-referrer-when-downgrade"
  src="https://www.google.com/maps/embed/v1/place?key=AIzaSyANx5ELozX0dIchLEQ7jAyVFV019xhsmeA&q=Space+Needle,Seattle+WA">
</iframe> -->
<script>
    var button1 = document.getElementById('button1');
    var button2 = document.getElementById('button2');
    var infoBox = document.getElementById('info-box');

    // Show info box on hover over Button 1
    button1.addEventListener('mouseover', function() {
        infoBox.style.display = 'block';
    });
    button1.addEventListener('mouseout', function() {
        infoBox.style.display = 'none';
    });

    // Change color on hover for Button 2
    button2.addEventListener('mouseover', function() {
        this.style.backgroundColor = 'rgba(0, 255, 0, 0.5)';
    });
    button2.addEventListener('mouseout', function() {
        this.style.backgroundColor = 'rgba(255, 255, 255, 0.5)';
    });

    // On click actions for both buttons
    button1.onclick = function() {
        alert('Button 1 clicked!');
    };
    button2.onclick = function() {
        alert('Button 2 clicked!');
    };
</script>


# World Map
<div style="position: relative; display: inline-block;">
    <img src="https://mirkoPortfolio.b-cdn.net/High-Resolution-World-Map-scaled.jpg" alt="World Map">
    <button id="button1" style="position: absolute; top: 20%; left: 17%; background-color: rgba(255, 255, 255, 0.5); border: 1px solid black; border-radius: 15px; padding: 4px 8px; cursor: pointer;">
        1
    </button>
    <button id="button2" style="position: absolute; top: 18%; left: 75%; background-color: rgba(255, 255, 255, 0.5); border: 1px solid black; border-radius: 15px; padding: 4px 8px; cursor: pointer;">
        2
    </button>
    <div id="info-box" style="display: none; position: absolute; top: 25%; left: 17%; background-color: white; border: 1px solid black; padding: 8px; border-radius: 5px;">
        Info about Button 1
    </div>
</div>

