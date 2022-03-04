This is the Idea that multiple views of the same data point can be used in creative ways to create tasks in [[Self-Supervised-Learning]].
For example consider the denoising task; in this task by converting a noisy *view* of a data point to its original *view*  we are effectively learning the **score** of data distribution [[@toshContrastiveLearningMultiview2021]]

Hint: Score was
$$
s(x) := \nabla_x \log p(x)
$$