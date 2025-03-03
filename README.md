# FootballVision AI: Precision Tracking and Performance Metrics

## Project Overview

This project aims to build an AI-powered football analysis system that can detect and track players, referees, and footballs in a video. By leveraging YOLO (You Only Look Once), one of the most advanced object detection models, we can accurately identify objects within each frame of the video. 

Additionally, the project incorporates several other technologies and algorithms to improve the analysis:

- **AI-Powered Object Tracking:** Use YOLO to detect and track players, referees, and footballs across frames.
- **Possession Time Measurement:** Calculate the percentage of time each team possesses the ball during the match.
- **Camera Motion Compensation:** Utilize optical flow to track camera movement and adjust perspective changes for more accurate tracking of players.
- **Depth Representation:** Apply perspective transformation to represent the field’s depth and convert measurements from pixels to real-world units (meters).
- **Player Performance Metrics:** Calculate speed and distance covered by players using tracking data and movement analysis.



![image](https://github.com/user-attachments/assets/30c7dc60-8e41-4e8c-8234-5ed2617396a7)


## Modules and Technologies Used

1. **YOLO for Real-time Detection:**
   - Detects and tracks players, referees, and the ball in video frames.
   - Known for fast and accurate object detection.

2. **KMeans Clustering for Team Identification:**
   - Segments image pixels to classify players based on shirt color.
   - Automatically assigns players to teams.

3. **Optical Flow for Camera Motion:**
   - Tracks and corrects camera movement between frames.
   - Improves tracking accuracy by compensating for motion.

4. **Perspective Transformation for Depth Adjustment:**
   - Adjusts the scene to simulate depth and scale.
   - Converts measurements from pixels to meters for real-world accuracy.

5. **Speed & Distance Calculation:**
   - Calculates player speed and distance covered using tracking data.
   - Combines player positions, camera movement, and perspective transformation.


## How to Run

1. Clone the repository:

   ```
   git clone https://github.com/xmadmaxdx/FootballVision-AI.git
   cd FootballVision-AI
   ```

2. Install the required dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Place the football match video file in the designated folder (`input_videos/video.mp4`).

4. Run the analysis script:

   ```
   python main.py
   ```

5. View the results in the `output_videos` folder where videos and analysis data will be saved.

## Demo Video

Watch the demo of the AI-powered football analysis system in action:

[Click here to watch the output video](https://drive.google.com/file/d/1DkIH1RPDXSx1m2Fut-qKE71-Rcp9lJ7s/view?usp=sharing)


## License

This project is licensed under the GNU GENERAL PUBLIC LICENSE Version 3.

## Conclusion

This project combines cutting-edge AI models and techniques such as YOLO for object detection, KMeans for color-based player classification, optical flow for camera motion adjustment, and perspective transformation for accurate real-world measurements. It's a powerful tool for analyzing football matches and tracking player performance in real-time. The system is highly adaptable and can be extended to other sports or video analysis applications.

## Future Work

- Improve the accuracy of player detection in different lighting conditions.
- Extend the system to support other sports like basketball or tennis.
- Integrate with additional datasets to improve the model's generalization across various football matches.
- Add more advanced tracking algorithms to handle occlusions or overlapping objects.
