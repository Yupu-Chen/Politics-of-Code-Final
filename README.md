# Machine Learning, Surveillance, and Public Safety

## Related Links

* **p5js sketch**: https://editor.p5js.org/Yupuuu/full/Lnl7LNdF8t
* **the Teachable Machine Model**: https://teachablemachine.withgoogle.com/models/KvnBxidt2/

## Background and Introduction of the Concept

This experimental mini research project is aimed at exploring the topics of machine learning, surveillance, and public safety. It is commonly known and detabed practice for the governments to use camera for surveillance and public security. In many countries, such as China and Singapore, the governments have recently adopted new cameras that integrated machine learning models for facial recognitions. This adoption was claimed to enhance public security by identifying recorded criminals and searching for suspects. However, this has raised concerns about privacy, discrimination, and arbitrary conviction. In making such a system, a great amount of facial data is needed, which requires residents and citizens to disclose much of their personal and biological infrormation to the authority. Moreover, the algorithms and models that analyze and classify the facial data could also discriminate people based on how they work. It is up to the training data and process whether the system would descriminate people. For example, there have been cases where African Americans are classified as inferior in the facial recognition models. Therefore, racial, cultural, and social identities can all be associated with the facial data, and the authority could easily abuse them when facial recognition is largely used in the widely dispersed security camera systems across the world.

It has to be admitted that cameras and facial recognition can indeed increase the public safety to a certain extent. In large-scale searching for suspects of crimes, surveillence cameras could be the key to accute and timely traces and locations of the suspects. Combined with machine learning and big data models, the survellance cameras could also predict potential public safety risks and inform police departments in advance. Given the advantages and challenges of the emerging applications of machine learning and surveillance in the name of public safety, it is important for the public to be aware of the privacy data collection process and its purposes and for the government to balance its need of public security and prevention from the abuse of public facial data and systematic biases.

## Technological Implementations

In developing the ideas and concept, I decide to produce a simplified version of the facial recognition model that could classfy people as potential protestors and non-protestors based on the training data I fed it.

Technologies involved:

* Teachable Machine, trained machine learning model for images based on MobileNet, a TensorFlow's computer vision model
* ML5, a p5js library that loads trained model to the p5js project, also based on TensorFlow
* P5js, to load the model and make interactive interface where the racial recognition result is displayed

Training data:

* Protestors: faces from the news reports online about protests and demonstrations (6 pictures)
* Non-protestors: faces from myself and my friends (6 pictures)

## Results and Findings



The training data are intetionally biased. One the one hand, the protestors' pictures are taken from news websites, which could have already been prejudicedly selected. On the other hand, the racial compositions of the two sets are not identical. In the set for protestors, the training data are almost entirely composed of white people. In the set for non-protestors, since I collected them from myself and people I know, the data are mostly Asians. Based on this, I predicted that this model would be very biased and most likely yield "Protest" for white people and "Non-Protest" for Asians. However, the result turned out differently.

The model works suprisingly well in my trials with different friends and images. With my friends, who as far I as know are not protestors and do not intend to become protestors in the near future, the model can successfully yield "Non-Protestor" result for almost 100% of the trials, regardless of my friends' races and appearances. Some people showed pictures of someone who is known to be protestors, and surprisingly the model could also accurately tell that they are protestors, again regardless of their races and appearances.

My limited knowledge on machine learning makes me unable to find out why this might happen, especially given that the amount of training is small in my mini project. But I suspect that it might happen as a result of the general model of the Teachable Machine. How the Teachable Machine works is that it is based on an existing trained model and replace the original training data with the customised ones. It is possible that the general model of the Teachable Machine already includes some features that could identify "common features" of protestors, if any.

## Discussion

While it is a mini experimental project that explores the very superficial level of machine learning, computer vision, and its application in public security, it has already shown some important lessons that we should be aware of when making more efforts into the exploitation of technology to promote social benefits. My training data reveal the practice of biases in feeding machine learning models, but results seem non-discriminatory. This can lead to a variety of inquiries into how biases in machine learning work, including their thresholds and social impact. Further manipulations and additions of training data might produce more interesting insights into how machine learning and big data could be better utilized to satisfy public safety needs without violating privacy and imposing excessive surveillance.





