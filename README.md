# Horse2zebra Challenge - CycleGAN with Segmentation-guided Attention

This project addresses the problem of unpaired image-to-image translation, specifically transforming horse images into zebra images. The core approach utilizes a CycleGAN[^1] architecture, enabling image translation without paired datasets and leveraging the concept of cycle consistency to ensure meaningful transformations. To enhance local feature detail, PatchGAN[^2] is employed as the discriminator, focusing on smaller patches of the image. 

**The novelty of this work lies in the incorporation of a segmentation-based attention mechanism**, which guides the generator to prioritize important regions of the image, ensuring more accurate and realistic translations. This attention mechanism not only improves translation quality but also helps avoid the unintended translation of irrelevant objects in the image, ensuring that only the horse undergoes the transformation. By focusing on key features, such as object boundaries and distinctive characteristics, the model preserves content while enhancing the overall fidelity of the generated images.
Through a series of experiments, promising results are observed, demonstrating effective translations between horse and zebra domains and showcasing the potential of this approach.

Full project report is available [here](https://github.com/LiorYaacov/Horse2zebra-Image-to-image-Translation/blob/main/Horse2zebra___Final_Project.pdf)

[^1]: Zhu, Jun-Yan, et al. "Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks." In *Computer Vision (ICCV), 2017 IEEE International Conference on*. 2017.  
[^2]: Isola, Phillip, et al. "Image-to-Image Translation with Conditional Adversarial Networks." 2018. [https://arxiv.org/abs/1611.07004](https://arxiv.org/abs/1611.07004)
