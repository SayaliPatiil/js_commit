const sdk = new Appwrite();

sdk
    .setEndpoint('https://[HOSTNAME_OR_IP]/v1') // Your API Endpoint
    .setProject('5df5acd0d48c2') // Your project ID
;

let promise = sdk.projects.updateTask('[PROJECT_ID]', '[TASK_ID]', '[NAME]', 'play', '', false, 'GET', 'https://example.com');

promise.then(function (response) {
    console.log(response); // Success
}, function (error) {
    console.log(error); // Failure
});