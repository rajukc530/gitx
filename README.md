<details>
<summary>Dropdown Heading</summary>
<br>
Choice 1
<br> Choice 2
<br> Choice 2
<br>
</details>

* [Deutsch](de/)
* [English](en/)


<div class="css-175oi2r"><div role="button" data-rnwi-handle="button" tabindex="0" class="css-175oi2r r-1i6wzkk r-lrvibr r-1loqt21 r-1otgn73 r-1awozwy r-42olwf r-rs99b7 r-18u37iz r-18kxxzh r-1777fci r-1ny4l3l r-z2wwpe r-mabqd8 r-1e081e0 r-14lw9ot r-1wgstfn r-1jsra8 r-1h9q8wt" style="transition-duration: 0.25s;" data-rnwi-1vckr1u-29dh1f-1jsra8-hover-focus="true"><div class="css-175oi2r r-1wbh5a2 r-11wrixw r-16y2uox"><div dir="auto" data-rnwi-handle="nearest" class="css-1rynq56 r-dnmrzs r-1udh08x r-1udbk01 r-3s2u2q r-1iln25a r-gg6oyi r-1b43r93 r-16dba41 r-hbpseb r-h7gdob">🇺🇸 English</div></div><svg viewBox="0 0 16 16" fill="none" preserveAspectRatio="xMidYMid meet" data-rnwi-handle="nearest" class="r-h7gdob r-1jkjb" style="vertical-align: middle; width: 16px; height: 16px;"><path fill-rule="evenodd" clip-rule="evenodd" d="M12.424 5.576a.6.6 0 010 .848l-4 4a.6.6 0 01-.848 0l-4-4a.6.6 0 01.848-.848L8 9.15l3.576-3.575a.6.6 0 01.848 0z" fill="currentColor"></path></svg></div></div>


<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.dropbtn {
  background-color: #3498DB;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}

.dropbtn:hover, .dropbtn:focus {
  background-color: #2980B9;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f1f1f1;
  min-width: 160px;
  overflow: auto;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown a:hover {background-color: #ddd;}

.show {display: block;}
</style>
</head>
<body>

<h2>Clickable Dropdown</h2>
<p>Click on the button to open the dropdown menu.</p>

<div class="dropdown">
  <button onclick="myFunction()" class="dropbtn">Dropdown</button>
  <div id="myDropdown" class="dropdown-content">
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </div>
</div>

<script>
/* When the user clicks on the button, 
toggle between hiding and showing the dropdown content */
function myFunction() {
  document.getElementById("myDropdown").classList.toggle("show");
}

// Close the dropdown if the user clicks outside of it
window.onclick = function(event) {
  if (!event.target.matches('.dropbtn')) {
    var dropdowns = document.getElementsByClassName("dropdown-content");
    var i;
    for (i = 0; i < dropdowns.length; i++) {
      var openDropdown = dropdowns[i];
      if (openDropdown.classList.contains('show')) {
        openDropdown.classList.remove('show');
      }
    }
  }
}
</script>

</body>
</html>
