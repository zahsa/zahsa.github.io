## Problems with Genrative Advarsarial Networks (GANs)


1. Training Instability

    GANs involve two neural networks (generator and discriminator) competing with each other.

    This adversarial setup can lead to non-converging or unstable training, where one network overpowers the other or they oscillate without improving.

    Training success depends on both networks learning at similar rates.

    If the discriminator becomes too strong or too week, the generator receives no useful feedback and it doesn't improve.
2. Mode Collapse

    The generator might find it easier to produce only a few types of outputs that fool the discriminator consistently.

    As a result, diversity in generated samples collapses, and it generates repetitive or limited outputs.

3. Difficulty in Evaluating Performance

    Unlike classification tasks with clear metrics like accuracy, measuring the quality of GAN outputs is difficult.

4. High Resource Requirements

    GANs often require large datasets, and significant compute

5. Sensitive to Hyperparameters and Architecture

    GANs are very sensitive to choices like learning rate, network design, batch size, etc.

    Even small changes can cause training to fail.


   
