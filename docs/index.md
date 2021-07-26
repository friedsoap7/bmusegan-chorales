<p class="switch-on-hover">
  <img class="hide-on-hover" src="figs/logo.png" alt="logo" style="max-width:200px;"/>
  <img class="show-on-hover" src="figs/logo_bmusegan.png" alt="logo" style="max-width:200px;"/>
</p>

[BinaryMuseGAN](https://salu133445.github.io/bmusegan/) is a follow-up project
of the [MuseGAN](https://salu133445.github.io/musegan/) project. In this
project, we first investigate how the real-valued piano-rolls generated by the
generator may lead to difficulties in training the discriminator for CNN-based
models. To overcome the binarization issue, we propose to append to the
generator an additional refiner network, which try to refine the real-valued
predictions generated by the pretrained generator to binary-valued ones. The
proposed model is able to directly generate binary-valued piano-rolls at test
time.

We trained the network with training data collected from
[Lakh Pianoroll Dataset](https://salu133445.github.io/lakh-pianoroll-dataset/).
We used the model to generate four-bar musical phrases consisting of eight
tracks: _Drums_, _Piano_, _Guitar_, _Bass_, _Ensemble_, _Reed_, _Synth Lead_ and
_Synth Pad_. Audio samples are available
[here](https://salu133445.github.io/bmusegan/results).