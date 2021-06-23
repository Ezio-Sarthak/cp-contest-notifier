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
