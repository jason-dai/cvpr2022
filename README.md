## End-to-End Big Data AI Pipeline Using Ray and Apache Spark
___

## Speaker
[Jason Dai](https://jason-dai.github.io/)

## Schedule
_7-10AM (Pacific Time), June 19, 2021_

## Description
As AI moves from experimentation to production, a key challenge in practice is how to seamlessly integrate distributed data processing and AI programs into a single unified pipeline. Today, AI researchers and data scientists usually need to go through a mountain of pains to apply AI models to production dataset that is stored in distributed Big Data cluster. Conventional approaches would set up two separate clusters, one for Big Data processing, and the other dedicated to deep learning and AI, with “connector” (or glue code) deployed in between. Unfortunately, this not only introduces a lot of data transfer overhead, but also requires additional efforts for managing separate workflows and systems in production.

To address these challenges, we have open sourced [Analytics Zoo](https://github.com/intel-analytics/analytics-zoo), which helps users to productionize their end-to-end Big Data AI pipelines in a distributed fashion. Using the [Orca](https://analytics-zoo.readthedocs.io/en/latest/doc/Orca/Overview/orca.html) library in Analytics Zoo, users can easily build data-parallel preprocessing (using existing Python libraries such as Pillow or OpenCV for images) for distributed dataset; and then within the same program, the users can directly apply AI models to the preprocessed data (that are partitioned and stored in-memory across large clusters), for transparently distributed training and inference through simple scikit-learn style APIs.

This tutorial will present the design patterns and tradeoffs for building end-to-end Big Data AI pipelines in production (with a focus on supporting computer vision models and workflow). In particular, it will describe how to seamlessly integrate Big Data and AI systems (such as Apache Spark and Ray) to support the distributed execution (for both data parallel preprocessing and AI programs), how to efficiently implement the distributed, in-memory data pipelines for these two logical systems (without expensive data transfer), and how to transparently combine different frameworks (such as Pillow, OpenCV, Pandas, Koalas, TensorFlow, PyTorch, Horovod, Ray Tune, OpenAI Baselines, etc.) into a single end-to-end workflow running on top of the underlying distributed execution environment. In addition, it will also share real-world experience and "war stories" of users who have adopted Orca to address their challenges when productionizing their end-to-end AI pipelines.

## Link
* Related [tutorial](https://jason-dai.github.io/cvpr2020/) at [CVPR 2018](http://cvpr2020.thecvf.com)
* Related [tutorial](https://jason-dai.github.io/aaai2019) at [AAAI 2019](https://aaai.org/Conferences/AAAI-19/aaai19tutorials/#sp2)