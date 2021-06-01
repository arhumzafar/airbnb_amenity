## Airbnb Amenity Detection

#### arhum zafar // 2021

this repository contains the work of a project to remake Airbnb's amenity detection using the [Detectron2](https://github.com/facebookresearch/detectron2) object-detection model from FacebookAI.

Amenity detection can be simply defined as object detection, but for common, everyday items. In this case, Airbnb uses detectron2 to identify items within a listing that a possible renter might want to know about. You can here more about the motivation behind this here: [Amenity Detection and Beyond](https://medium.com/airbnb-engineering/amenity-detection-and-beyond-new-frontiers-of-computer-vision-at-airbnb-144a4441b72e).

#### App

I used [Streamlit](https://streamlit.io/) to deploy a live app that runs the model. (*I ran the app for a couple days but then took it down due to costs of running & mantaining it --- A fun follow up would be to find a way to deploy the model again, but with little to no costs).*

#### Repo Contents

- In the repository, notebooks numbered 0-10 are all different steps taken to load and process the images and train the model. 

- `preprocessing.py`contains the functions to take the [images in our dataset](https://storage.googleapis.com/openimages/web/index.html) and convert them in a form that is [Detectron2 style](https://detectron2.readthedocs.io/tutorials/datasets.html).
