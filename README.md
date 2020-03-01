# Custom Ghost Blog Theme

Based off the default Casper Ghost theme, this is our customized blog theme. Feel free to use it, under the condition that you remove *all* references to our company.

# Local Dev Setup

Ghost has built an excellent, easy to use local dev setup. Follow their initial setup instructions, and run `ghost start`. For the instructions below, we'll assume you created your ghost setup in a folder simply named `ghost`.

http://localhost:2368/ should now show you the default Casper theme, and the admin log is located at http://localhost:2368/ghost/

To get this custom theme up and running:

- `ghost stop`
- cd to `/ghost/content/themes` and clone this theme
- cd into the `bloglc` folder (which was just created by your clone command) and then `yarn install`
- cd back up to your main `ghost` folder
- `ghost start`
- Visit http://localhost:2368/ghost/ and create a new admin account. Then set the following vlaues; note that they should be specific to your company/organization:
  - Title = Name of your company
  - Description = A short description; this will be displayed near the top of the homepage of your blog
  - Set an Icon and Logo
  - *Delete* the publication cover image
  - Set link to your Facebook page (if you have none, you'll need to edit the template to remove links to this)
  - The navigation links on the Design page are *not* functional. For various reasons which you can read about in the source, we've hardcoded the navbar link URLs
  - Finally, at the bottom of the Design page, set `bloglc` as the active theme!


