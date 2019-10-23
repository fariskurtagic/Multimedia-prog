function openPage(pageName, elmnt, color) {
    // Hide all elements with class="tabcontent" by default */
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }

    // Remove the background color of all tablinks/buttons
    tablinks = document.getElementsByClassName("tablink");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].style.backgroundColor = "";
    }

    // Show the specific tab content
    document.getElementById(pageName).style.display = "block";

    // Add the specific color to the button used to open the tab content
    elmnt.style.backgroundColor = color;
    
}

$(document).ready(function(){
    $('[data-toggle="popover"]').popover(); 
});

$(document).ready(function(){

// Activate Carousel with a specified interval
    $("#Dali").carousel({interval: false});
// Activate Carousel with a specified interval
    $("#Gogh").carousel({interval: false});
// Activate Carousel with a specified interval
    $("#Monet").carousel({interval: false});
    
});