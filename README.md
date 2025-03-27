# Satellite_Image_Segmentation_for_building_detection_using-_Adversial_Residual_U-Net_based_Model
### THEME
The project revolves around leveraging advanced machine learning techniques and IoT technology for precise building detection in satellite imagery. By integrating a U-Net-based Generative Adversarial Network (GAN) model with Raspberry Pi IoT systems, the project aims to develop a sophisticated solution that uses publicly available satellite datasets to enhance the accuracy and real-time capabilities of building detection. This approach seeks to offer innovative tools for applications such as urban planning, disaster management, and environmental monitoring, addressing the needs of government agencies, companies, and other stakeholders involved in smart city and infrastructure initiatives.

#### INTRODUCTION
In our project, "Satellite Image Segmentation for Building Detection Using an Adversarial Residual U-Net Model," we present a cutting-edge solution that integrates advanced machine learning techniques with IoT technology to enhance building detection accuracy from satellite imagery. Utilizing an Adversarial Residual U-Net model, our approach combines the powerful encoder-decoder structure of U-Net with residual learning to improve feature extraction and mitigate the vanishing gradient problem. The adversarial training framework further refines the model's ability to generate realistic and precise segmentation maps. This innovative model is deployed on Raspberry Pi IoT devices, enabling real-time data processing and analysis in remote and resource-constrained environments. By leveraging publicly available satellite image datasets, our solution is both accessible and cost-effective, ensuring broad applicability across various geographical regions. The integration of these technologies addresses the technical challenges of building detection, offering significant improvements in precision and robustness. Our project has practical applications in urban planning, disaster management, and environmental monitoring, providing a powerful tool for government agencies, companies, and other high-level stakeholders. The anticipated impact of our project includes better urban infrastructure management, enhanced disaster response capabilities, and more effective environmental conservation efforts.

![image](https://github.com/user-attachments/assets/ced5372b-377a-4465-b14a-fa59a75263e2)

###   SIMPLIFIED SCHEMATIC OF U-NET BASED GAN MODEL

![image](https://github.com/user-attachments/assets/e0cfad3f-385b-4c78-b639-29c34a743490)

### ADVERSIAL RESIDUAL U-NET BASED MODEL

-->This model combines the strengths of U-Net for segmentation with the adversarial learning framework of a Generative Adversarial Network (GAN) and the robustness of residual connections to enhance the learning process.

-->U-Net Backbone for Segmentation:

1.Contracting Path (Encoder): Extracts deep features from the satellite images.

2.Expansive Path (Decoder): Reconstructs pixel-level predictions for buildings in the images.

3.Skip Connections:  Directly connect layers from the encoder to the decoder to preserve spatial information.

-->U-Net Architecture:

1.Encoder Path (down-sampling) with convolution or involution blocks.

2.Bottleneck Layer: A deep layer that uses the involution layer with a high number of channels for capturing deeper features.

3.Decoder Path (up-sampling) where the spatial resolution is gradually restored, making use of skip connections to preserve finer details.

-->The output layer uses a 1x1 convolution to produce the final segmentation map, with sigmoid activation for binary segmentation (e.g., building vs. non-building).

## INVOLUTIONAL LAYER
The involution layer is an improved type of layer in neural networks that helps with image tasks, like detecting buildings in satellite images.

Custom Focus on Each Area: Unlike regular layers that use the same filter across an image, involution layers create unique filters for each spot. This makes the model pay more attention to details in each specific part of the image.

Fewer Parameters Needed: Since involution layers don’t need to use as many shared filters, they end up with fewer parameters, making the model smaller and more efficient.

 Great for Segmentation: In tasks like segmentation (separating areas in an image), these layers capture detailed differences better. For example, they can help detect individual buildings more accurately.
 
Efficient for Low-Power Devices: Since they use fewer resources, involution layers are ideal for devices like the Raspberry Pi, which have limited processing power.

Better at Recognizing Complex Patterns: They can detect complicated details in an image better than regular layers, making them helpful for analyzing dense or cluttered areas in satellite images.

![image](https://github.com/user-attachments/assets/f5f04ce2-abfc-46dc-9133-4d90f433930b)

### MATHEMATICAL TERMINOLOGIES IN ML USED IN THIS PROJECT

![image](https://github.com/user-attachments/assets/e5438cc6-a7f0-4719-9d06-515b5742329f)

### DATASETS GATHERING
Space-Net ,Kaggle, Google Earth Engine, ISRO Bhuvan platform datasets especially for Indian urban datsets  are the popular datasets used for various machine learning and deep learning tasks.

### MATHEMATICAL RESULTS DURING TRAINING 

Implemented U-net based model and calculated the values of dice coefficent,IOU,Prescion score,recall,accuracy.(Dice Coefficient: 0.7891 IoU: 0.6517 Precision Score: 0.8111 Recall: 0.7683 Accuracy: 0.8980)

### TRAINING RESULTS WITH INDIAN CITIES

![image](https://github.com/user-attachments/assets/8d8ea3e4-7f7d-4364-a53d-d05617e609fe)

### TESTING THE MODEL WITH REAL TIME DATA (My college pics)

![image](https://github.com/user-attachments/assets/64924b44-66a2-4a5b-99b2-6104fe2f4124)

### HARDWARE IMPLEMENTATION
  #  1.IOT ARCHITECTURAL FLOW
  ![image](https://github.com/user-attachments/assets/4fd70fa9-46c8-4b7a-b0a2-a1fa713f0579)

  # 2.TOOLS USED

1.RVNC viewer: It allows users to access and control computers remotely from anywhere, making it ideal for managing devices, accessing files, or running applications without being physically present.

2.Advanced IP Scanner: It is typically used for network tasks, and its mention in the context of satellite image segmentation may be a misunderstanding or typo(typographical error).

3.PuTTY: It is primarily used for secure remote access to servers and network devices through SSH, Telnet, and other protocols, making it a crucial tool for system administrators.

4.Hexa(drone): A hexacopter is a six-rotor drone offering enhanced stability, redundancy, and payload capacity, making it ideal for aerial photography, mapping, and industrial applications. Its design allows continued flight even if one motor fails, ensuring reliability in various conditions. 


















