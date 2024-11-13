# Hand Gesture Recognition Model for Smart Home Control

This project uses computer vision to recognize hand gestures, which can be used to control smart home devices like lights, fans, and media players. Developed using Google’s Teachable Machine, the model recognizes a set of predefined gestures that can be customized to control various devices or perform specific actions within a smart home environment.

## Project Overview
The goal of this project is to build a robust and reliable hand gesture recognition model. This model serves as a prototype for controlling smart devices in real-time through simple gestures. With further optimization, this model can contribute significantly to accessible technology, providing hands-free control options for individuals with mobility impairments or those in need of convenience.

---

## Data Collection and Preparation

### Data Collection Process
The dataset was created by capturing images and videos of various hand gestures in diverse lighting conditions, backgrounds, and angles. The goal was to capture gestures like **wave, thumbs-up, palm open, and fist**, as well as other gestures relevant to smart home control.

To ensure the dataset was comprehensive and minimized bias, images were collected from different individuals with varying skin tones and hand shapes. Diverse backgrounds and lighting conditions were used to make the model more robust and less sensitive to specific conditions.

### Data Preparation
The captured images were labeled according to gesture type and processed to normalize image size and resolution. To improve model performance, data augmentation techniques (like flipping, rotating, and cropping) were applied to expand the dataset further. This pre-processing aimed to make the model more reliable by simulating real-world scenarios and ensuring accuracy.

**Impact on Model Performance**  
The diversity of the dataset led to increased accuracy and reliability, as the model performed well in varying real-world conditions without overfitting to any specific hand, background, or lighting type. This comprehensive dataset made the model more adaptable to dynamic environments.

---

## Model Creation Using Google’s Teachable Machine

Google’s Teachable Machine was used for model development. This tool simplifies the process of building image recognition models by allowing users to upload datasets directly and train models without coding. The steps to create the model are as follows:

1. **Dataset Upload**: All labeled images were uploaded into Teachable Machine’s interface and categorized by gesture type.
2. **Training Configuration**: Teachable Machine offers options to configure training settings like batch size, epochs, and learning rate. Optimal parameters were selected based on initial testing to balance accuracy and training time.
3. **Training and Exporting the Model**: After training, the model was exported in TensorFlow Lite format for compatibility with mobile and IoT devices, as well as a WebGL format for browser-based applications.

---

## Features and Functionalities

The model includes the following features and functionalities:

- **Real-time Gesture Recognition**: Detects predefined gestures in real-time using a device camera.
- **Device Control Integration**: Gesture recognition can be mapped to smart home controls. For example, a thumbs-up gesture could turn on the lights, while a wave gesture could adjust fan speed.
- **Customizable Gestures**: Users can retrain or adjust the model to recognize new gestures as needed, allowing flexibility for various control needs.
- **Mobile and IoT Compatibility**: The model is optimized for TensorFlow Lite, making it compatible with edge devices and mobile platforms, ideal for use in smart home setups.

---

## Model Evaluation

### Evaluation Methods
The model’s performance was evaluated using:

- **Accuracy and Precision**: Measured the model’s ability to correctly identify gestures from real-world test data.
- **Cross-Validation**: The dataset was split into training and validation sets, with a test set used to measure the model’s generalization ability.
- **Confusion Matrix**: Used to analyze which gestures were frequently misclassified, helping us refine the model by adding more data for underperforming gestures.

### Results
The model achieved a high accuracy of over 90% for most gestures, showing reliable performance across various lighting conditions and backgrounds. Evaluation results indicated that the model could handle minor variations in hand position and orientation, though certain gestures with similar hand shapes occasionally required additional training data to improve differentiation.

---

## Applications and Real-World Use Cases

This model is a step towards hands-free control interfaces, which can enhance accessibility and convenience. Some real-world applications include:

- **Smart Home Control**: Adjust lighting, control fans, or play/pause media with simple hand gestures.
- **Accessibility Aid**: For individuals with physical disabilities, this model offers a non-contact method for controlling smart home devices.
- **Touchless Interfaces**: In hygiene-sensitive environments, gesture-based controls eliminate the need for physical touch.
- **Automation Systems**: Integrate gesture recognition with smart home systems (like Alexa or Google Home) for seamless, automated control.

---

## Project Demo

Below are screenshots from the project demo:

![Real-time Gesture Detection](./screenshots/gesture_detection.png)
*Screenshot showing real-time gesture detection in action.*

![Teachable Machine Training](./screenshots/teachable_machine_training.png)
*Screenshot of the training interface on Google’s Teachable Machine.*

![Smart Home Control Setup](./screenshots/smart_home_control.png)
*Screenshot showing integration with smart home control panel.*

---

## Conclusion

This hand gesture recognition model lays the groundwork for innovative, accessible technology in smart homes. With further development, this model can support a wider range of gestures and applications, creating more inclusive and adaptable control solutions for a variety of environments.

For any questions or contributions, please reach out to the project maintainer.

---

## Screenshort
<img width="362" alt="Screenshot 2024-11-12 at 9 53 36 PM" src="https://github.com/user-attachments/assets/83132d96-aabe-49ae-b240-be90b101ed54">


<img width="314" alt="Screenshot 2024-11-12 at 9 28 20 PM" src="https://github.com/user-attachments/assets/c9220fb5-bc36-4a23-93d3-9ffca8d43bcc">
