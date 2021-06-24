# cp-contest-notifier
A firefox extension that provides details of upcoming CP contests from platforms like CodeForces, CodeChef and AtCoder.

<p align="center">
  <img src="https://user-images.githubusercontent.com/55916430/123145777-cd46cd00-d47a-11eb-9ad5-f93736ed41bf.png">
</p>


## Use case
To add this extension to firefox, you'd just have to add a `credentials.json` file in your local clone, that includes username and api key values as received from [CLIST](https://clist.by) website login/signup.

The format of credentials should be `JSON`:

```code
{
  "username": "clist_username_here",
  "api_key": "clist_api_key_here"
}
```

NOTE: Follow the naming **strictly** to avoid pushing the credentials to git.

## Adding add-on to firefox permanently

To use the add-on on a daily basis, you'd need to install the add-on permanently. Follow the below steps for the same:

1. First add `manifest.json` file as a temporary addon in firefox, by navigating to `debug:debugging`.
2. Note the `Extension ID` value and copy-paste its value to `id` parameter of `gecko` under `browser_specific_settings` in `manifest.json`
3. Now wrap the required extension files in a `.zip` or `.xpi` file. (The compressed file should contain `mainfest.json`, `credentials.json`, `icons/` dir, `popup.html` and `popup.js`).
4. Now add this compressed file as add-on by going to `Extensions` -> `Settings icon` -> `Install add-on from file`.

Now you're good to go!
