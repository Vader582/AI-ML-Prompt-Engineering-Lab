# [AI Desk Object Sorter]
## Project Description
This project uses Google's Teachable Machine to classify four common objects found on my desk.

## Classes Identified
List the objects your model was trained to identify:
* Class 1 (Pens)
* Class 2 (Scissors)
* Class 3 (Mugs)
* Class 4 (Screwdrivers)

## Discussion & Reflection

1.  **Model Performance & Iteration:**
    * How accurate was your first trained model?
      
 I started with Pens and Scissors and took about fifty pictures of each. I used three pens and one pair of scissors. Initially, the first model was confused by scissors. The model could identify pens relatively well, but would, at certain angles, think the scissors were pens.
 
    * What steps did you take to iterate and improve its performance? (e.g., added more images, diversified image types for a specific class). 
    
To improve the performance, I took fifty additional photos of each type of item. I also added additional types of pens and scissors to the pool to add variation. At this point, I also decided to add two more classes to the experiment, the mugs and screwdrivers. 

    * How did these changes affect the model's accuracy and confidence scores?
    
The model’s accuracy improved when I added additional photos. The model seemed to have much more confidence in its predictions than when I first started. At certain angles, there is still some confusion in the model regarding scissors. Additionally, if the scissors are not open, the model will often mistake them for pens.

2.  **Challenges & Observations:**
    * Which objects were the easiest for your model to learn and distinguish? Why do you think that was?
      
Pens and mugs are the easiest for the model to identify. I believe the pen’s simple shape was what made it easy to recognize.  The mugs, due to their handles, were easier for the model to identify.

    * Which objects were the most challenging? What made them difficult (e.g., similar shapes, variable appearances)?
    
The scissors and screwdrivers were the most challenging. I added the screwdrivers to try to confuse the model. That was precisely what occurred. The similar shape of the screwdrivers to pens often confused the model. Unless the scissors were open, the model often thought they were pens. The model could benefit from additional background variations. Although I did change this somewhat, it may not have been sufficient to assist the model in making correct identifications. I also chose varying color schemes for each item scanned, but it did not assist in the recognition.

    * What happened when you showed the model an object it wasn't trained on? How did the confidence scores behave, and why is this significant?
    
When shown items that were not in any class, the model often predicted they were pens. Items like a rock or a remote control, despite usually not being shaped like a pen, were identified by the model as a pen. The model was nearly 100% confident that these misinterpreted items were pens. Were this a more critical AI vision model, such incorrect decisions could lead to poor outcomes.

3.  **Bias in AI:**
    * If you only trained your "mug" class with images of *your specific mug* (and didn't vary color, shape, etc.), how well do you think it would recognize other students' significantly different mugs? How does this illustrate the concept of bias being introduced through training data?
      
The model would not predict these well. I attempted to confuse my model with unidentified mugs. The model was somewhat confused by them. The confidence in its answers was not as high. Training the model on my specific mug may also lead to overfitting, as it may not learn the concept of a mug in general. The limited exposure to one or two mugs gives the model a very narrow view of mugs, thus illustrating the concept of bias.

    * Imagine all your training images were taken in very bright, direct lighting. What might happen if you tried to use the model in a dimly lit room or with strong shadows? How does this relate to the robustness and potential biases of AI models?
    
This would add confusion to the AI model. Bad data in, gets bad data out. Images in dimly lit rooms would be harder for the model to interpret. The model would be very confident in photos from brightly lit rooms, but images from the darker rooms could be misdiagnosed, leading to bias against those types of class items.

4.  **Model Limitations & Usefulness:**
    * What are some key limitations of the model you created?
      
The model is limited in its interpretations due to the scope of what it has been exposed to. It seems to identify items somewhat easily that it’s already seen but variations can confuse it.

    * Why is it useful to be able to download your trained model files (like `model.json`, `weights.bin`) and share them (e.g., via GitHub)? What does this enable?
      
Being able to share the files allows others to test your model under varied conditions and see if it maintains its accuracy. Downloaded these files can also act as a preservation of the data at that particular time.

5.  **Real-World Applications & Ethics:**
    * Brainstorm 2-3 real-world applications where a similar image classification model could be useful.
      
Image classification is already used to separate produce, good items from bad or small from larger. Also, Ford uses image classification in their truck factories to judge the quality of the paint jobs and identify issues before leaving the factory.
https://www.designnews.com/automotive-engineering/fords-kentucky-truck-plant-embraces-ai-3d-printing-for-enhanced-vehicle-production


    * Briefly discuss one ethical consideration that developers should keep in mind when building and deploying image recognition AI in the real world (e.g., related to fairness, privacy, misuse).
   
Privacy is a genuine concern. We want to expose models to as much information as possible, but people need the ability to opt out of being lumped into the data sharing.

## (Optional) Challenges Faced / Interesting Discoveries
* Add any other specific challenges you encountered or interesting things you discovered during this lab.
  
I thoroughly enjoyed this lab. 
I was surprised at my model’s confusion with scissors. I figured the handles would be enough to help the AI identify them correctly. 
I wish I had used a different camera, something other than my MacBook webcam. It limited how I took pictures and where. My hand and head were often in the sample photos. I’m sure this also skewed the data and recognition ability.

## (Optional) Screenshot
* You can embed a screenshot of your Teachable Machine interface here if you like.
 
<img width="1588" alt="final lab screenshot" src="https://github.com/user-attachments/assets/c5cf5c7c-2c06-470f-8e10-22cf5152e0eb" />
