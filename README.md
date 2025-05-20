Ethan Kook - A18092777
1) I would run the tests in the Github action that runs whenever code is pushed. This is so everytime someone pushes a change, they can first test the code before merging.
2) I would not use E2E testing to test whether a function returns the correct output because a smaller, more specific test would work better than testing a users actions from the beginning to the end. 
3) Navigation mode analyzes the page right after it loads while snapshot analyzes it in its current state. 
4) Based on the lighthouse results, properly sizing images can potentially save 518KiB and serving images in next-gen formats such as WebP and AVIF, which often provide better compression than PNG or JPEG, can potentially save 165KiB. We can also add a `<meta name="viewport">` tag, which optimizes the app for mobile screen sizes, and also prevents a 300 millisecond delay to user input. 

Screenshot of test results: /ResultsScreenshot.png
