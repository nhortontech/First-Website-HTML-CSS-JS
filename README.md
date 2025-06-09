# First-Website-HTML-CSS-JS
My first attempt at building a website with HTML, CSS and JS


Go through tutorial and each part of code to break down (ie box icons and their use) https://boxicons.com/?query=menu 


Errors ran into and fixed:

Common forgetting to save all before reloading localhost

Not displaying local host - installed open-in-browser extension

Spelling mistake in “font-size” causing font not to change size on website


Was missing : in this - min-height: 100vh;

Had a space between ‘ ‘ when meant to be no space like: btn-box .btn::before {


Coloru of box was not background color and then itneracting with mous hover to slide red, was stuck on red because:
.btn-box .btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0%;
    height: 100%;
    background: red;
    z-index: -1;
    transition: .5s;

Width had to be set to 0, was on 100% originally

Error displaying images on webpage with css - ended up being due to my URL not going another layer into source folder, needed the .. at start of url to go into project folder, and them images…was just looking for image in project folder at beginning

.home {
    display: flex;
    align-items: center;
    padding: 0 9%;
    background: url('../images/home.jpg') no-repeat;
    background-size: 50%;
    background-position: center;
}

Had to recreate background image to match color hexz code




Error relating to css formatting of webpage. All information was shifted underneath each other and on left hand side rather than centred and spit into two sections like so:
.education {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    min-height: auto;
    padding-bottom: 5rem;
}


.education .education-row {
    display: flex;
    flex-wrap: wrap;
    gap: 5rem;
}




FIX: I read other syntax for wrap and adjusted “wrap” under .education-row section to “nowrap” for result:


Adjusting margins and font sizes caused similar issue: 

.education-row .education-column {
    flex: 1 1 60rem;
}


.education-column .title {
    font-size: 2.5rem;
    margin: 0 0 1.5rem 2rem;
}





Fixed by adjusting the flex to 1 1 112rem;





.education-row .education-column {
    flex: 1 1 112rem;
}


.education-column .title {
    font-size: 2.5rem;
    margin: 0 0 1.5rem 2rem;
}

I had to then change flex to 165 after adjusting font-size for boxes


Error: formatting of contact form



FIX: typo in code, line 506 of css page typed “centre” instead of “center”



ERROR: contact page was not centered


