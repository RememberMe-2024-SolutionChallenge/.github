## **0. Introduction**

RememVR is a service facilitating participation in reminiscence therapy based on VR contents for dementia patients. Our team implemented video-to-VR technology based on AI models, which proves to be significantly more cost-effective than other equipment commonly employed in the creation of existing VR content.

[![Demo Video](https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/video.png)]("YOUTUBE_LINK")

> You can check out the Demo Video by clicking above image.

## **1. Problem Statement**

#### **Main Target**

Dementia patients and caregivers are the main target of our challenge.

#### **Problem Context**

According to WHO, there are over 55 million people worldwide living with dementia in 2020 and they project this number will almost double every 20 years. Aged society and increasing amount of people with dementia implies that care technology should back up the status quo. Reminiscence therapy is one of the effective therapy for people diagnosed with dementia, enhanced with VR contents. However, creating VR content with realistic models of objects and people involves a costly process that includes 3D scanning and real-time rendering. A recent Korean documentary 'Meeting You' has shown similar VR experience with our service. The total project costed about $120px,000 and the cost only for the VR contents was half of the total production cost.

#### **Main Problem**

RememVR is designed to mitigate the expensive process involved in creating VR content for reminiscence therapy.

## **2. UN Sustainable Development Goal & Targets**

<img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/sdgs.png" style="width: 70%;">

We chose UN Sustainable Development Goal 3, specifically with target 3.8 and 3.d. As dementia is a disease that influences whole community which includes individuals and their family, our service could provide essential health care services. Simultaneously, providing VR contents based on reminiscence therapy would strengthen the capacity for risk reduction and management of dementia.

## **3. Key Features**

We separated our application into two tracks, caregiver and care recipient tracks are those. Caregivers can make VR scenes and care recipients can experience VR scenes engaging in reminiscence therapy. 

<img src="https://github.com/RememVR-2024-SolutionChallenge/.github/blob/main/profile/assets/care_main.png?raw=true" style="width: 50%;">

### a. Key Features in Caregiver Track

#### (1) Creating Avatar
RememVR generates avatars representing the patient's cherished individuals. These avatars, combined with place VR scene, offer the patient an immersive recollection of memories. RememVR assists in safeguarding the continuity of the patient's memories. Caregivers can upload a video featuring the person whom they like to transform into an avatar.

<img src="https://github.com/RememVR-2024-SolutionChallenge/.github/blob/main/profile/assets/caregiver%20-%201.png?raw=true" style="width: 50%;">

#### (2) Creating VR Scene (Place)
RememVR creates VR experiences encapsulating the places intertwined with a patient's memories. We all live with our unique sense of places, as visiting specific locations can evoke memories from particular times. Places in VR will make them feel as if they are physically present in that space. Caregivers can upload videos that showcase distinctive features of the location if its indoor. If with outdoor features they can select the specific location. 

<img src="https://github.com/RememVR-2024-SolutionChallenge/.github/blob/main/profile/assets/caregiver%20-%202.png?raw=true" style="width: 50%;">

#### (3) Creating VR Scene (Avatar + Place)
Caregivers can select one or two avatars, and one place VR scene to build a completed VR scene. After VR scene is generated, care recipient can find out that scene in his/her VR experience list.

<img src="https://github.com/RememVR-2024-SolutionChallenge/.github/blob/main/profile/assets/caregiver%20-%203.png?raw=true" style="width: 50%;">

### b. Key Features in Caregiver Track

#### (1) VR Experience
Care recipients can participate in VR scene. Our character ‘Brainy’ helps care recipient to follow the steps for VR experience which is a part of the reminiscence therapy. 

<img src="[https://github.com/RememVR-2024-SolutionChallenge/.github/blob/main/profile/assets/care%20recipient%20-%201.png?raw=true" style="width: 30%;">

#### (2) Badge Tracker
After the care recipient completes the VR experience, badges are awarded as p![image](https://github.com/RememVR-2024-SolutionChallenge/.github/assets/123253883/a0d39746-771a-47ed-a3d9-1f66b7dfd412)
art of gamification. These badges can be viewed not only on the Care Recipient's home-page but also on the Caregiver's home. There are a total of three badge designs, and one of them is randomly assigned.

<img src="https://github.com/RememVR-2024-SolutionChallenge/.github/blob/main/profile/assets/care%20recipient%20-%202.png?raw=true" style="width: 50%;">

## **4. Architecture**

<img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/architecture.jpg" style="width: 90%;">

> _Detailed descriptions of each component are provided in their respective repositories._

- **Client:** [Mobile Application](https://github.com/RememVR-2024-SolutionChallenge/RememVR-client) [VR viewer](https://github.com/RememVR-2024-SolutionChallenge/vr-viewer)
- **Server:** [Gateway/Application server](https://github.com/RememVR-2024-SolutionChallenge/gateway-server) [AI server](https://github.com/RememVR-2024-SolutionChallenge/ai-server)
- **Other server utils:** [AI task scheduler](https://github.com/RememVR-2024-SolutionChallenge/AI-task-scheduler) [Realtime DB synchronizer](https://github.com/RememVR-2024-SolutionChallenge/realtime-DB-synchronization)

## **5. How to Run**
> _This project is developed using Flutter. You can launch this app by downloading an apk file or running with IDE(VSCode)!_
> 
### Download APK

1. Enter https://github.com/RememVR-2024-SolutionChallenge/RememVR-client/releases
2. Click the latest release
3. Download app-release.apk
4. Launch this app on Android devices.
   
### Run with IDE

 Before you start, make sure you have installed the following on your system:

- Flutter SDK
- VS Code
- Dart and Flutter extensions for VS Code
- Android emulator or physical device

1. Clone the RememVR repository from GitHub: https://github.com/RememVR-2024-SolutionChallenge/RememVR-client.git
2. Open the project folder in VS Code.
3. In VS Code, open the command palette (View > Command Palette) and type "Flutter: Run Flutter Doctor". This will check your system to make sure everything is set up correctly.
4. In VS Code, open the main.dart file and click the "Run" button. This will launch the app in the emulator or on your physical device.


## **6. Team Members**

| [GuiJung Woo](https://github.com/woog2roid)<br/>BE Engineer                                                                                              | [SeoYeon Byun](https://github.com/seooyxx)<br/>AI Engineer                                                                                             | [Seoyoung Kim](https://github.com/seoyoung723)<br/>PM / Designer                                                                                           | [JinWoo Choi](https://github.com/ryan00102)<br/>FE Engineer                                                                                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/woog2roid.png" style="width: 120px"> | <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/seooyxx.png" style="width: 120px"> | <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/seoyoung723.png" style="width: 120px"> | <img src="https://raw.githubusercontent.com/RememVR-2024-SolutionChallenge/.github/main/profile/assets/contributors/ryan00102.png" style="width: 120px"> |

We are team **RememVR** from _Google Developer Student Clubs Korea University, Seoul Campus_.
