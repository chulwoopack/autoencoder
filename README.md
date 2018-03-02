# Autoencoder

This repo is for developing an angorithm for Autoencoder.

## Manifold Hypothesis
우리가 보는 데이터들(이미지 데이터들)이 사실은 더 작은 벡터 공간안에 살고있다 라는 이야기.
(데이터들이 살고 있는공간: manifold)

# Variational Autoencoder

Encoder '''p(z|x), actually q(z|x)'''
Decoder '''p(x|z)'''

## Reparameterization trick
latent variable z가 random variable이기 때문에, sampling을 해야하는데, sampling은 미분 불가라 gradient를 구할 수 없다.
따라서, 마치 z 자신은 deterministic한데, 외부에서 random noise e이 입력되는 것처럼 바꿔버린다.

## KL-divergence
흔히 regularizer라고 부르는데, 
'''얼마나 많은 정보가 손실되는가'''

## E
흔히 (negative) reconstruction loss라고 부르는데,
'''얼마나 출력값이 입력값을 잘 따라가는가'''

## Resources
VAE: https://jamiekang.github.io/2017/05/21/auto-encoding-variational-bayes/