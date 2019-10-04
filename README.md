# The Keras Model Zoo
Ready to go, downloadable models for Keras

```
                               .-----------------._,,
                               |      KERAS      (_")=
                               |      MODEL       |||                __
                               |  🐆  ZOO   🐅   ||#\_____       .-/  \
                        ssgg   |------------------|\# # # #\    .''  ..'----,_
                   ____SG ..]  |       |/         | \##_#_#/\ =:.'-\         )\
                ,-( _   SS(_9)_|      _(")        | |/|/\|\|   ::   |  ,_   /  `
               / (_____;-.____;;    o(_,\\        | I I  I I    `   [|_/\\_]
```
hosted with :heart: from Infinite Red


| Model | Description | Model Specifics | Additional Info |
| ----- | ----------- | --------------- | --------------- |
| [Food 101](https://s3.amazonaws.com/ir_public/ai/keras-zoo/food_101.h5) |  Identify 101 different types of food from a single 299x299 image | Input: [, 299, 299, 3] - Output: Softmax index of food: 101 values | [Details](./info/Food101/README.md) |
| [Dog and Cat Faces](https://s3.amazonaws.com/ir_public/ai/keras-zoo/dnc_faces.h5) | Find those cute dog and cat faces in any photo | Input: RGB tensor - Output: Normalized (0 to 1) 4 corners of the pet face | [Examples](./info/Dog_and_Cat_faces/README.md) |


## How to Contribute

### Hosting the Model
**We will host the model file.** Do a pull request with your updates and a link to your model. During review we will download and host your model on our S3 so you can update your pull request URL to one that we will host.  You simply need to find a way to get your model in our hands temporarily and we'll take on the hosting for the repo.

### Your Pull Request
Update the README.md to have all the information on your provided model.  Then add a folder in the `/info` section that includes credit, examples, and more friendly information on your trained keras model.
