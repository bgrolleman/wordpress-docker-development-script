This is a wordpress develoment environment that uses Docker to build a test setup 
to run code against.

I mostly wanted a very simple setup that would use the official mysql and wordpress
containers and that would use my current directory as theme root.

If you do not change the dev file then the wp-content/themes/wpdev and
wp-content/plugins/wpdev point to your local environment.

In short, . is mounted as /srv in docker and symlink is setup to point to this
directory.

Feedback welcome


## Usage
1. Copy "dev" to your project (theme/plugin dir)
2. Update dev variables to have the right name
3. Run "./dev setup"
4. Connect to http://localhost:8080
5. When done "./dev stop"
6. If you want to start again, use "./dev start"

