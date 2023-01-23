# Representations and Abstractions

### [Deep Affordance Foresight: Planning Through What Can Be Done in the Future](http://arxiv.org/abs/2011.08424)

Planning in realistic environments requires searching in large planning spaces. Affordances are a powerful concept to simplify this search, because they model what actions can be successful in a given situation. However, the classical notion of affordance is not suitable for long horizon planning because it only informs the robot about the immediate outcome of actions instead of what actions are best for achieving a long-term goal. In this paper, we introduce a new affordance representation that enables the robot to reason about the long-term effects of actions through modeling what actions are afforded in the future, thereby informing the robot the best actions to take next to achieve a task goal. Based on the new representation, we develop a learning-to-plan method, Deep Affordance Foresight (DAF), that learns partial environment models of affordances of parameterized motor skills through trial-and-error. We evaluate DAF on two challenging manipulation domains and show that it can effectively learn to carry out multi-step tasks, share learned affordance representations among different tasks, and learn to plan with high-dimensional image inputs.


### [Continuous Relaxation of Symbolic Planner for One-Shot Imitation Learning](http://arxiv.org/abs/1908.06769)

We address one-shot imitation learning, where the goal is to execute a previously unseen task based on a single demonstration. While there has been exciting progress in this direction, most of the approaches still require a few hundred tasks for meta-training, which limits the scalability of the approaches. Our main contribution is to formulate one-shot imitation learning as a symbolic planning problem along with the symbol grounding problem. This formulation disentangles the policy execution from the inter-task generalization and leads to better data efficiency. The key technical challenge is that the symbol grounding is prone to error with limited training data and leads to subsequent symbolic planning failures. We address this challenge by proposing a continuous relaxation of the discrete symbolic planner that directly plans on the probabilistic outputs of the symbol grounding model. Our continuous relaxation of the planner can still leverage the information contained in the probabilistic symbol grounding and significantly improve over the baseline planner for the one-shot imitation learning tasks without using large training data.


### [Adversarial Skill Networks: Unsupervised Robot Skill Learning from Video](https://arxiv.org/abs/1910.09430)

Key challenges for the deployment of reinforcement learning (RL) agents in the real world are the discovery, representation and reuse of skills in the absence of a reward function. To this end, we propose a novel approach to learn a task-agnostic skill embedding space from unlabeled multi-view videos. Our method learns a general skill embedding independently from the task context by using an adversarial loss. We combine a metric learning loss, which utilizes temporal video coherence to learn a state representation, with an entropy regularized adversarial skill-transfer loss. The metric learning loss learns a disentangled representation by attracting simultaneous viewpoints of the same observations and repelling visually similar frames from temporal neighbors. The adversarial skill-transfer loss enhances re-usability of learned skill embeddings over multiple task domains. We show that the learned embedding enables training of continuous control policies to solve novel tasks that require the interpolation of previously seen skills. Our extensive evaluation with both simulation and real world data demonstrates the effectiveness of our method in learning transferable skills from unlabeled interaction videos and composing them for new tasks.


### [Bottom-Up Skill Discovery from Unsegmented Demonstrations for Long-Horizon Robot Manipulation](http://arxiv.org/abs/2109.13841)

We tackle real-world long-horizon robot manipulation tasks through skill discovery. We present a bottom-up approach to learning a library of reusable skills from unsegmented demonstrations and use these skills to synthesize prolonged robot behaviors. Our method starts with constructing a hierarchical task structure from each demonstration through agglomerative clustering. From the task structures of multi-task demonstrations, we identify skills based on the recurring patterns and train goal-conditioned sensorimotor policies with hierarchical imitation learning. Finally, we train a meta controller to compose these skills to solve long-horizon manipulation tasks. The entire model can be trained on a small set of human demonstrations collected within 30 minutes without further annotations, making it amendable to real-world deployment. We systematically evaluated our method in simulation environments and on a real robot. Our method has shown superior performance over state-of-the-art imitation learning methods in multi-stage manipulation tasks. Furthermore, skills discovered from multi-task demonstrations boost the average task success by 8% compared to those discovered from individual tasks.


### [R3M: A Universal Visual Representation for Robot Manipulation](https://arxiv.org/abs/2203.12601)

We study how visual representations pre-trained on diverse human video data can enable data-efficient learning of downstream robotic manipulation tasks. Concretely, we pre-train a visual representation using the Ego4D human video dataset using a combination of time-contrastive learning, video-language alignment, and an L1 penalty to encourage sparse and compact representations. The resulting representation, R3M, can be used as a frozen perception module for downstream policy learning. Across a suite of 12 simulated robot manipulation tasks, we find that R3M improves task success by over 20% compared to training from scratch and by over 10% compared to state-of-the-art visual representations like CLIP and MoCo. Furthermore, R3M enables a Franka Emika Panda arm to learn a range of manipulation tasks in a real, cluttered apartment given just 20 demonstrations.


### [Real-World Robot Learning with Masked Visual Pre-training](https://arxiv.org/abs/2210.03109)

In this work, we explore self-supervised visual pre-training on images from diverse, in-the-wild videos for real-world robotic tasks. Like prior work, our visual representations are pre-trained via a masked autoencoder (MAE), frozen, and then passed into a learnable control module. Unlike prior work, we show that the pre-trained representations are effective across a range of real-world robotic tasks and embodiments. We find that our encoder consistently outperforms CLIP (up to 75%), supervised ImageNet pre-training (up to 81%), and training from scratch (up to 81%). Finally, we train a 307M parameter vision transformer on a massive collection of 4.5M images from the Internet and egocentric videos, and demonstrate clearly the benefits of scaling visual pre-training for robot learning.