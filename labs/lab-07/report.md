# Checkpoint 1
Built using the commands cmake -G "Unix Makefiles" ../cmake and make -j5
![image](https://user-images.githubusercontent.com/60018973/159052817-bbe30e86-f85c-480f-a927-6ba180707dc3.png)

# Checkpoint 2
- Find the Nightly and Experimental sections and look at some of the submissions. How can you see what tests were run for a particular submission?
    - Click on the number(s) under the test category of the table, and it will lead you to a page that shows all the tests that were run.

- Find a submission with errors. Can you see what the error condition was? How does this help you debug the failure?
    - I checked the first failed test in the Nightly section. The error condition was: Result is [Bus error], not [1]. stderr does not match that expected. This helps debug the failure as it tells the user what was expected in the command vs. what was given that lead to an error.

- Find a system that is close to your specific configuration in the Nightly, Nightly Expected or one of the Masters sections. How clean is the dashboard? Are there any errors that you need to be concerned with?
    - I checked terfin.kitware under the Nightly Expected section. The dashboard is relatively clean, with only 1 test error in the current build and no errors elsewhere. The error seems to report that permission to open one of the files for testing was denied, however all other tests passed.

![image](https://user-images.githubusercontent.com/60018973/159528205-aeeb866b-3cfd-418a-b77d-0b2a1e2c3b9f.png)


# Checkpoint 3
![image](https://user-images.githubusercontent.com/60018973/159525537-596c46fa-8084-4da1-8292-73b8d35735d6.png)

Fix:
<br>![image](https://user-images.githubusercontent.com/60018973/159528103-b335bfab-9b8f-4c25-adaf-d57606350f21.png)
![image](https://user-images.githubusercontent.com/60018973/159528885-b68d1236-2235-4df8-99b6-7f6f6d06bc4e.png)

# Checkpoint 4
Repository link: https://github.com/kimdo20/lab7
![image](https://user-images.githubusercontent.com/60018973/159546320-38e55e87-5676-4e80-86c3-d02b7128bd36.png)
![image](https://user-images.githubusercontent.com/60018973/159546778-a3be86a6-5dfc-4637-9df5-90ff91e8c37f.png)
