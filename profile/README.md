## **0. Introduction**

RememVR is a service facilitating participation in reminiscence therapy based on VR contents for dementia patients. Our team implemented video-to-VR technology based on AI models, which proves to be significantly more cost-effective than other equipment commonly employed in the creation of existing VR content.

[![Demo Video](https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/video.png)]("https://youtu.be/SvhOM7ff8sI")

> You can check out the Demo Video by clicking above image.

## **1. UN Sustainable Development Goal & Targets**

<img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/sdgs.png" style="width: 70%;">

We chose UN Sustainable Development Goal 3, specifically with target 3.8 and 3.d. As dementia is a disease that influences whole community which includes individuals and their family, our service could provide essential health care services. Simultaneously, providing VR contents based on reminiscence therapy would strengthen the capacity for risk reduction and management of dementia.

## **2. Key Features**

We separated our application into two tracks, caregiver and care recipient tracks are those. Caregivers can make VR scenes and care recipients can experience VR scenes engaging in reminiscence therapy.

### a. Key Features in Caregiver Track

- **(1) Creating VR Scene (Place)**
  - RememVR creates VR experiences encapsulating the places intertwined with a patient's memories. We all live with our unique sense of places, as visiting specific locations can evoke memories from particular times. Places in VR will make them feel as if they are physically present in that space. Caregivers can upload videos showcasing distinctive features of the location if it's indoor, forward-faced, or unbounded.
- **(2) Creating Avatar**
  - RememVR gives avatars representing the patient's cherished individuals. These avatars, combined with place VR scene, offer the patient an immersive recollection of memories. RememVR assists in safeguarding the continuity of the patient's memories. Caregivers can upload a video or an image featuring the person whom they like to transform into an avatar.
- **(3) Creating VR Scene (Avatar + Place)**
  - Caregivers can select avatars, and a VR scene to build a completed VR scene. After VR scene is generated, care recipient can find out that scene in his/her VR experience list.

### b. Key Features in Care recipient Track

- **(1) VR Experience**
  - Care recipients can participate in VR scene. Our character ‘Brainy’ helps care recipient to follow the steps for VR experience which is a part of the reminiscence therapy.
- **(2) Badge Tracker**
  - After the care recipient completes the VR experience, badges are awarded as part of gamification. These badges can be viewed not only on the Care Recipient's home-page but also on the Caregiver's home. There are a total of three badge designs, and one of them is randomly assigned.

## **3. How to Run**

> _This service is developed mobile and VR device. Below are the methods for installing the application on mobile devices and running it on VR devices._

### Install Mobile Application

#### Method 1. Download APK

1. Enter [https://github.com/RememVR-2024-SolutionChallenge/RememVR-client/releases](https://github.com/RememVR-2024-SolutionChallenge/RememVR-client/releases).
2. Click the `latest` release.
3. Download `app-release.apk`.
4. Launch this app on Android devices.

#### Method 2. Run with IDE

Before you start, make sure you have installed the following on your system: `Flutter SDK`, `VS Code`, `Dart and Flutter extensions for VS Code`, `Android emulator or physical device`

1. Clone the RememVR repository from GitHub:
   ```
   git clone https://github.com/RememVR-2024-SolutionChallenge/RememVR-client.git
   ```
2. Open the project folder in VS Code.
3. In VS Code, open the command palette (View > Command Palette) and type "Flutter: Run Flutter Doctor". This will check your system to make sure everything is set up correctly.
4. In VS Code, open the main.dart file and click the "Run" button. This will launch the app in the emulator or on your physical device.

### Run VR Devices

Experience our VR viewer if you have a VR setup. Before launching the app, ensure your VR and mobile devices are connected.

#### 😎 For Quest 2 Users:

1. **Connecting your Quest 2**: Link your Quest2 with mobile device. Follow the instructions in-VR and in the Meta Quest mobile app to complete the setup process. Refer to the [official guidance](https://www.meta.com/ko-kr/help/quest/articles/getting-started/getting-started-with-quest-2/install-meta-quest-mobile-app/). Just ensuring a mirroring connection suffices for our service.

   ❗Note: Your VR device and mobile device **MUST BE** connected with same network.

2. **Accessing the VR Viewer**: Once connected, the `Start VR` button on our web-based VR viewer becomes automatically accessible. Click it, and enjoy your VR journey!

   - Access several pre-trained example models [here](https://rememvr-2024-solutionchallenge.github.io/vr-viewer/demo).
   - This VR viewer connects with Flutter APK. If you have your own trained scene and avatar, you can see your own model with this viewer. [Learn how to create your own model here](https://github.com/RememVR-2024-SolutionChallenge/ai-server).
   - We've tested with Oculus Quest 2 and Galaxy S22. We will support more VR devices soon.

## **4. Architecture**

<img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/architecture.jpg" style="width: 90%;">

> _Detailed descriptions of each component are provided in their respective repositories._

- **Client: [Mobile Application](https://github.com/RememVR-2024-SolutionChallenge/RememVR-client) [VR viewer](https://github.com/RememVR-2024-SolutionChallenge/vr-viewer)**
- **Server: [Gateway/Application server](https://github.com/RememVR-2024-SolutionChallenge/gateway-server) [AI server](https://github.com/RememVR-2024-SolutionChallenge/ai-server)**
- **Other server utils: [AI task scheduler](https://github.com/RememVR-2024-SolutionChallenge/AI-task-scheduler) [Realtime DB synchronizer](https://github.com/RememVR-2024-SolutionChallenge/realtime-DB-synchronization)**

## **5. Team Members**

| [GuiJung Woo](https://github.com/woog2roid)<br/>BE Engineer                                                                                              | [SeoYeon Byun](https://github.com/seooyxx)<br/>AI Engineer                                                                                             | [Seoyoung Kim](https://github.com/seoyoung723)<br/>PM / Designer                                                                                           | [JinWoo Choi](https://github.com/ryan00102)<br/>FE Engineer                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/woog2roid.png" style="width: 120px"> | <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/seooyxx.png" style="width: 120px"> | <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/seoyoung723.png" style="width: 120px"> | <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/ryan00102.png" style="width: 120px"> |

We are team **RememVR** from _Google Developer Student Clubs Korea University, Seoul Campus_.
