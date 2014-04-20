# WPI Running Club Website
This is the source code for the WPI Running Club website. It is statically built with Jekyll and pushed to the WPI servers.

## How to build the static site
You will need jekyll, which in Debian and Ubuntu can be had with just 'apt-get install jekyll'.

From the website directory...

    jekyll build

Replace with your account info.

    sftp sjkelly@ccc.wpi.edu

In the CCC shell run.

    cd /home/running
    put -r public_html/

And the website should now be live on the WPI servers.
It would be uber awesome to automate this with a git hook using ssh keys.

## Adding routes
First set the map on mapmyrun to be public. When you click on the link to view the map there will be a number at the end of the URL. For example, http://www.mapmyrun.com/routes/view/393742172. Add this number with a hyphen under 'route_id' in the HTML file for the corresponsing difficulty like below.

    route_id:
        - 281937637
        - 282197493
        - 386899162

## Group Account Links

* http://www.wpi.edu/+groupaccount
* http://www.wpi.edu/+gred

