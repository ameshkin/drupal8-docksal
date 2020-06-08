# Docksal with Drupal 8 Starter

Simple Drupal 8 Installation with Docksal, bootstrap and SASS with Barrio theme

Features:

- Drupal 8
- Bootstrap Barrio and SASS
- Docker with Docksal


## Project setup

1. Clone this repo into your Projects directory

    ```
    git clone https://github.com/ameshkin/drupal8-docksal.git
    cd drupal8
    ```

2. Initialize the site

    This will initialize local settings and install the site via drush

    ```
    fin init
    ```

3. Point your browser to

    ```
    http://drupal8.docksal
    ```

When the automated install is complete the command line output will display the admin username and password.


4. Project Login

You need to log into the bash script and get a one time user login for drupal.

`
fin bash;
cd docroot;
drush uli;
`

Then paste this url into the browser replacing `default` with your hostname.


5. Activate Theme

Install bootstrap_sass theme by navigating to `http://drupal8.docksal/admin/appearance`

6. NPM Install

You will need to install the npm packages and run gulp from your sub theme folder.

`docroot/themes/bootstrap_barrio/subtheme/bootstrap_sass`

`
npm install;
gulp styles;
`

## Issues

You will need to make sure port 80 is open.
