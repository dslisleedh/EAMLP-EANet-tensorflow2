<h1>
Beyond Self-attention: External Attention using Two Linear Layers for Visual Tasks

[arXiv](https://arxiv.org/abs/2105.02358)
</h1>

<h3>
요약 :  

Self-Attention을 Linear layer로 해석함.  Simplified SA는 O = I * softmax(I * I^t)임. 이런식으로 Attention을 하면 각 개체에서 특징적인 부분을 가져올 순 있지만, 
Object Detection에서 요구하는 것 처럼 한 Category 내에서 유지되는 특징을 가져오는 것은 힘듦.  
  
그럼 자기 자신을 2번 곱하는 대신, Memory block을 2번 곱하는 방식으로 구현됨. Memory block은 Dense layer와 동일하나 bias가 없으며, Dense layer기에 전체 Data에서 뽑아낸 특징들을 
보유할 수 있음. 
</h3>

<h6>
앵간하면 실제로 사용해보는데, 너무 이해가 안되서 External Attention, Multi-Head External Attention 구현하고 넘어감. 나중에 기회가 되면 구현 해볼 것임.
</h6>
