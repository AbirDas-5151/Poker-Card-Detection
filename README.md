# Poker Hand Detection Using YOLO and OpenCV

This project uses **YOLO object detection** to recognize playing cards in real time through a webcam and determines the poker hand based on the detected cards. It combines the power of deep learning for card detection and custom poker hand logic to evaluate the hand.

---

## 🚀 **Features**
- **Real-Time Card Detection**: Detects individual playing cards from a live webcam feed.
- **Poker Hand Evaluation**: Identifies the poker hand (e.g., "Full House," "Straight Flush") using the detected cards.
- **Customizable Detection**: Trained with a custom YOLO model (`playingCards.pt`) specifically for card recognition.
- **Interactive Display**: Displays bounding boxes, card names, and hand evaluation results directly on the video feed.

---

## 🛠️ **Technologies Used**
1. **Programming Language**: Python
2. **Libraries**:
   - OpenCV: For video processing and visualization.
   - YOLO (from `ultralytics`): For object detection.
   - cvzone: For enhanced visualization (e.g., bounding boxes, text overlays).
   - Custom Poker Hand Function: Implements poker hand evaluation logic.

---

## 📋 **Setup Instructions**

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/poker-hand-detection.git
cd poker-hand-detection
```

### 2. Install Dependencies
Ensure you have Python 3.7+ installed. Then, install the required libraries:
```bash
pip install ultralytics opencv-python cvzone
```

### 3. Prepare YOLO Weights
Download the custom YOLO model weights (`playingCards.pt`) trained for card detection. Place the file in the project directory.

### 4. Run the Program
Start the poker hand detection system:
```bash
python poker_hand_detection.py
```

---

## 📂 **Project Files**
- `poker_hand_detection.py`: Main script for detecting cards and evaluating poker hands.
- `playingCards.pt`: YOLO model trained on playing cards.
- `PokerHandFunction.py`: Contains the logic to evaluate poker hands (e.g., "Flush," "Two Pair").
- Additional required files: Webcam or video input for live detection.

---

## 🎯 **How It Works**
1. **Card Detection**:
   - Uses YOLO to detect cards in the webcam feed.
   - Classifies cards into suits and ranks (e.g., "10H" for 10 of Hearts).

2. **Building the Hand**:
   - Tracks detected cards and forms a "hand" of up to 5 unique cards.

3. **Poker Hand Evaluation**:
   - Calls `PokerHandFunction.findPokerHand(hand)` to evaluate the type of poker hand.

4. **Display Results**:
   - Draws bounding boxes around detected cards.
   - Displays the detected cards and evaluated poker hand on the video feed.

---

## ⚙️ **Customization**
- **Add New Features**: Expand the `PokerHandFunction` module to support more card games or custom rules.
- **Confidence Threshold**: Adjust the confidence threshold (default: 0.5) for card detection accuracy.
- **Graphics**: Add custom overlays for an enhanced user interface.

---

## 📊 **Potential Applications**
- Teaching poker rules and hand evaluation.
- Card game monitoring systems.
- Fun, interactive demonstrations of AI in gaming.

---

## 🤝 **Contributions**
Contributions are welcome! Here’s how you can contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

---

## 📜 **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 📧 **Contact**
For questions or feedback, feel free to reach out:
- **Email**: addyabir111@gmail.com.com
- **GitHub**: [AbirDas-5151](https://github.com/AbirDas-5151)

---

## 📝 **Acknowledgments**
- **Ultralytics YOLO**: For state-of-the-art object detection.
- **cvzone**: For simplifying visualization in OpenCV.
- **Poker Hand Logic**: Custom algorithm for poker hand evaluation.

Happy coding and enjoy playing poker with AI! 😊
