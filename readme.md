# CircleCI w/ Parallelization
#### [Made by Shawn Harris with Scribe](https://scribehow.com/shared/CircleCI_w_Parallelization__97Vv94EfS4iGYpnXF9OhMQ)


**1. Navigate to your terminal:**
```
mkdir .circleci
cd .circleci/
touch config.yml
```

**In your config.yml add the parallelization example from our docs (minus npm run start, if it's not applicable): https://docs.cypress.io/guides/continuous-integration/circleci#Parallelization**

**After adding your .yml script, in your terminal:**
```
cd ..
git add .
git commit -am "add circleci .yml"
git push origin YOUR_BRANCH
```

![](https://colony-recorder.s3.amazonaws.com/files/2023-03-16/6dd8da8e-cf3a-4965-b891-d1a7c0721844/stack_animation.webp)

**2. Navigate to https://app.circleci.com/pipelines**
**Click "Organization Settings"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/35d55ee7-fddc-4a7c-8a56-df9b740152be/ascreenshot.jpeg?tl_px=0,156&amp;br_px=746,576&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=51,139)

**3. Click "Security"**<br />
**Click "Yes" to allow Cypress community orb**

![](https://colony-recorder.s3.amazonaws.com/files/2023-03-16/4aee9b38-a031-4a85-aa00-42ad4ff5587a/stack_animation.webp)

**4. Navigate back to https://app.circleci.com/pipelines**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/53e56bde-1347-459a-95da-484ddc0aca4e/user_cropped_screenshot.jpeg?tl_px=0,0&amp;br_px=746,420&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=5,17)

**5. If you connected using GitHub, click "Set Up Project" after locating the correct repo.**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/ec35ca96-61b3-463e-84cd-8cbc8b624dbb/user_cropped_screenshot.jpeg?tl_px=892,117&amp;br_px=1638,537&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=397,139)

**6. Click "Fastest" (We already set up the config and pushed to GitHub in step 1)**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/7e87e2d1-8449-4551-aca6-13bcd4497b79/user_cropped_screenshot.jpeg?tl_px=291,0&amp;br_px=1037,420&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=262,123)

**7. Click "Set Up Project"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/e81aa589-7675-492b-a4d4-372bb5a2792b/ascreenshot.jpeg?tl_px=756,380&amp;br_px=1502,800&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=262,139)

**8. Navigate to https://cloud.cypress.io**
**Click "YOUR_PROJECT"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/e0ed4fca-f15f-43f7-8948-6ee43567e3f6/user_cropped_screenshot.jpeg?tl_px=250,4&amp;br_px=996,424&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=262,139)

**9. Click "Project Settings"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/03850c81-493f-49c4-b48d-88df7f85e3ff/ascreenshot.jpeg?tl_px=0,433&amp;br_px=746,853&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=84,139)

**10. Copy "Record Key" and "Project Id" to clipboard**
**Click here**

![](https://colony-recorder.s3.amazonaws.com/files/2023-03-17/946f54c0-cd18-4122-9cff-7149dfeefc5b/stack_animation.webp)

**11. Navigate back to https://app.circleci.com/pipelines/**
**Click "YOUR_PROJECT"**
**Click "Project Settings"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/086f8b2c-5ce7-4681-915e-71ae7cd819cf/ascreenshot.jpeg?tl_px=1173,123&amp;br_px=1919,543&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=467,139)

**12. Click "Environment Variables"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/57adc797-bdb3-4fbe-8d98-8090bada8539/ascreenshot.jpeg?tl_px=0,181&amp;br_px=746,601&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=51,139)

**13. Click "Add Environment Variable"**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/7373ba9a-4bab-4c8b-bd67-82f05f075208/ascreenshot.jpeg?tl_px=295,238&amp;br_px=1041,658&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=262,139)

**14. Add "CYPRESS_RECORD_KEY" and "CYPRESS_PROJECT_ID" environment variables**

![](https://ajeuwbhvhr.cloudimg.io/colony-recorder.s3.amazonaws.com/files/2023-03-16/29518918-66b2-4f34-8b42-35a259a64704/ascreenshot.jpeg?tl_px=415,305&amp;br_px=1161,725&amp;sharp=0.8&amp;width=560&amp;wat_scale=50&amp;wat=1&amp;wat_opacity=1&amp;wat_gravity=northwest&amp;wat_url=https://colony-recorder.s3.amazonaws.com/images/watermarks/28e69b_standard.png&amp;wat_pad=262,139)

**15. Navigate back to terminal:**
```
git commit --allow-empty -m "Trigger build"
git push origin YOUR_BRANCH
```