<script>
    import githubLogo from '$lib/assests/connect-logos/github-mark.png';
    import linkedinLogo from '$lib/assests/connect-logos/LI-In-Bug.png';
</script>

<div id="footer">
    <div _ngcontent-jvr-c39="" class="squiggle"><svg _ngcontent-jvr-c39="" aria-hidden="true" width="100%" height="8" fill="none" xmlns="http://www.w3.org/2000/svg"><pattern _ngcontent-jvr-c39="" id="a" width="91" height="8" patternUnits="userSpaceOnUse"><g _ngcontent-jvr-c39="" clip-path="url(#clip0_2426_11367)"><path _ngcontent-jvr-c39="" d="M114 4c-5.067 4.667-10.133 4.667-15.2 0S88.667-.667 83.6 4 73.467 8.667 68.4 4 58.267-.667 53.2 4 43.067 8.667 38 4 27.867-.667 22.8 4 12.667 8.667 7.6 4-2.533-.667-7.6 4s-10.133 4.667-15.2 0S-32.933-.667-38 4s-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0-10.133-4.667-15.2 0-10.133 4.667-15.2 0" stroke="darkgrey" stroke-linecap="square"></path></g></pattern><rect _ngcontent-jvr-c39="" width="100%" height="100%" fill="url(#a)"></rect></svg></div>
    <div id="content" class="grid grid-cols-3 p-4">
        <div class="col-span-2 flex justify-start">
            <a href="https://github.com/aditya24raj" target="_blank" rel="noreferrer"><img class="logo" src={githubLogo} alt="github-logo"/></a>
            <a href="https://www.linkedin.com/in/aditya24raj" target="_blank" rel="noreferrer"><img class="logo" src={linkedinLogo} alt="linkedin-logo"/></a>
        </div>
        <div>
            Developed with ❤️ by aditya raj
        </div>
    </div>

</div>

<style>
    #footer {
        margin-top: 100px;
    
    }
    #content {
        color: grey;
        text-align: end;
    }

    .logo {
        max-height: 20px;
        margin-right: 10px;
        display: inline-block;
        text-align: left;
    }
</style>