# Air-Canvas
Air Canvas is an interactive drawing project using color detection and motion tracking. Users draw in the air, captured by a camera, translating movements into a virtual canvas. Features include color selection, brush thickness adjustment, and an engaging platform for artistic expression.

**Key Components:**

- **1 Camera Input   :**   The project utilizes a camera (such as a webcam) to capture live video input. This video feed serves as the basis for tracking movements.
- **2 Color Detection:** The system identifies a specific color (marker) or hand movements in the video feed to track the user's input. Color thresholds are used to distinguish                            thedrawing tool from the background.
- **3 Drawing Logic  :** When the marker or hand movements are detected, the system translates those movements into drawing commands on a virtual canvas. This involves updating                            the canvas with each frame based on the tracked position.
- **4 Canvas Display :** The virtual canvas is displayed in real-time, allowing users to see their drawings as they create them. The canvas could be a window on a computer screen                           or projected onto a larger surface.
- **5 Interactive Features:** Users can interact with the Air Canvas through additional features, such as changing colors, adjusting brush thickness, or even selecting different                                 drawing tools.

**User Interaction:**

- **Color Selection :** Users can change the drawing color by interacting with a color palette or by pointing the marker to a specific color region in the environment.
- **Brush Thickness :** The thickness of the drawing tool can be adjusted, providing flexibility in creating various artistic effects.
- **Eraser Mode     :** Some implementations include an eraser mode, allowing users to erase specific parts of their drawings.
- **Gesture Controls:** Advanced versions might incorporate gesture controls for additional functionalities, such as undo, redo, or switching between drawing tools.

 **ALGORITHMS:**

1. **Color Detection:**
   - **Algorithm:** HSV Color Thresholding
   - **Description:** Convert the video frame from BGR to HSV color space and apply thresholding to identify a specific color (marker) or hand movements. This helps isolate the drawing tool from the background.

2. **Object Tracking:**
   - **Algorithm:** Contour Detection and Object Tracking
   - **Description:** Use contour detection to identify the region of interest (ROI) in the frame, such as the marker or hand. Object tracking algorithms, like centroid tracking, can be employed to track the position of the detected object across frames.

3. **Drawing on Canvas:**
   - **Algorithm:** Real-time Drawing Logic
   - **Description:** Continuously update a virtual canvas based on the tracked position of the marker or hand. Algorithms handle the logic to draw lines, shapes, or strokes in real-time, creating a smooth and interactive drawing experience.

4. **Color Selection:**
   - **Algorithm:** Pixel Color Analysis
   - **Description:** Allow users to change drawing colors by analyzing the color of pixels at the clicked or pointed location. This involves sampling the color of a pixel from the video feed and updating the drawing tool's color accordingly.

5. **Interactive Features:**
   - **Algorithm:** User Interaction Logic
   - **Description:** Implement algorithms for interactive features, such as adjusting brush thickness, erasing, or changing drawing tools. These algorithms interpret user input and modify the drawing parameters accordingly.
  
6. **Gesture Controls:**
   - **Algorithm:** Gesture Recognition
   - **Description:** Advanced versions may include gesture recognition algorithms to interpret specific hand gestures for additional functionalities like undo, redo, or switching between drawing tools.

7. **Background Subtraction (Optional):**
   - **Algorithm:** Background Subtraction
   - **Description:** In more advanced setups, background subtraction algorithms can be employed to isolate the moving object (marker or hand) from the background, enhancing the accuracy of object detection.

8. **User Interface (UI):**
   - **Algorithm:** UI Interaction Logic
   - **Description:** Implement algorithms to handle user interface interactions, such as button clicks for color palette selection or adjusting brush thickness. These algorithms contribute to the overall user experience.

These algorithms collectively enable the Air Canvas to track user movements, interpret input, and dynamically update the virtual canvas, providing an interactive and engaging platform for digital drawing. The specific implementation may vary based on project requirements and the complexity of desired features.

**Applications:**

- **Artistic Expression:** Air Canvas provides a unique and engaging platform for artistic expression, enabling users to create digital artwork in an intuitive and immersive                                  manner.
- **Education:**           It can be used as an educational tool to teach basic principles of computer vision and image processing, making learning more interactive and fun.
- **Entertainment:**       Air Canvas can serve as an entertaining interactive installation in public spaces, events, or museums, captivating audiences and encouraging                                        participation.
- **Therapeutic Use:**     The project could be adapted for therapeutic purposes, allowing users to engage in a creative and stress-relieving activity.
