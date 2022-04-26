## Signatures for Brands on a Mission

### How to install

1.  Drop the folder on a web server that can be used to serve content to the
    web.

    This is so that the icons and logos can keep being used. They need to be
    downloadable from web when people want to display your email. The web server for
    <brandsonamission.com> could be good.

    For local iteration, you can trivially serve it with a simple python server:

    ```sh
    $ cd $THIS_DIRECTORY
    $ python3 -m http.server
    ```

2.  Note the path where this directory is served, that I will designate
    as `$BASEURL` in the rest of the instructions.

    It could be for example <brandsonamission.com/signatures/> (or
    <localhost:8000/> for a local server).

3.  In `signature.html`, replace `.` in the image addresses by the value of
    `$BASEURL`.

    For example:

    ```html
    <img src="./boam_logo.png" />
    ```

    Should become:

    ```html
    <img src="brandsonamission.com/signatures/boam_logo.png" />
    ```

4.  Render <signature.html> in a browser window, then

    1. Select all the page's content (`Ctrl/Cmd` + `A`) and copy it.

    2. Paste it in the signature edit field of Outlook or Gmail or whichever
       email client you are using.

    3. Change the name and job title as needed. Don't touch anything else.

    4. Try to send an email, and verify that it renders well on mobile and
       desktop. If it doesn't, you probably should look into some professional
       tool that handles whatever you're doing properly.

Good luck! Designing email signature sucks.
- Christina's pocket developer
