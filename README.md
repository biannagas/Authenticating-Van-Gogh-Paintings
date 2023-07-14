# Authenticating Van Gogh Paintings using Convolutional Neural Networks
![the-starry-night-over-the-rhone](https://github.com/biannagas/Phase-4-Project/assets/131709766/49395235-2f84-4a97-af9d-b76916913cc9)

# Business Problem
About half of all fine art in global circulation is suspected to be fraudulent. The art industry is estimated to generate $60+ billion annually, implying that the forgery industry is worth around $30+ billion. Art forgery is the third-highest grossing criminal enterprise of the last 40 years.

Van Gogh is one of the most popular Post-Impressionist painters and a prime target for forgeries. Even with
expert analysis, it is hard for people to distinguish fakes, as seen when nine paintings previously designated as fakes have been determined to be real Van Gogh works.

I aim to use machine learning image classification models to better analyze and predict true Van Gogh paintings
from forgeries, imitations, and even AI generated version of his art.

# Data Understanding
The original dataset contained 8,400+ artworks from the top 50 artists in art history, of which 877 were Van Gogh paintings. The model was also trained on AI generated Van Gogh art, Van Gogh replica paintings and Van Gogh style imitation paintings. The primary nationality of the artists was French and most painted in Impressionist or Post-Impressionism styles. The dataset was sampled to only keep a similar amount of non-Van Gogh artworks.

<img width="487" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/ffc591ea-2359-4fc7-8e1c-7874f3603e4b">

<img width="482" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/26727a30-e811-45e2-b4dd-9619d49153a5">

<img width="482" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/7060e444-0438-45a6-a505-4e9fa12ee1a1">

The following is shows the differing rgb pixel distributions for a Van Gogh painting, an AI generated painting and a painting by the artist caravaggio. The model will use the differing pixel information to try to distinguish the paintings from one another.

<img width="393" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/7aab30d4-c8c4-47dd-9f26-770c4a9360ab">

<img width="358" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/3088cb7e-0cc6-4350-a17a-183c3b4eaa8e">

<img width="425" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/ed4c82de-9203-454a-8d39-34e754f2d534">

# Results 
The best Image Classification model was 53% accurate when determining non-Van Gogh paintings and 45% accurate when determining Van Gogh paintings.

The best model had 2 convolutional layers and 4 dense layers. I also tried adding dropout rate in another model as well as a VGG16 model but the initial model had the best confusion matrix.

According to the confusion matrix, the model primarily had trouble overclassifying non-Van Gogh art as being one of his paintings. 

<img width="472" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/80cef457-a6db-4541-a3d8-7ad6db12e0b7">

<img width="299" alt="image" src="https://github.com/biannagas/Phase-4-Project/assets/131709766/789eb25c-dcdd-4d0b-aa3a-8853e5c8ee2e">



