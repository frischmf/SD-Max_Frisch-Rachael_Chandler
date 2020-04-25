# Final Self-Assessment

## Maximilian Frisch

I contributed the majority of the software and hardware implementation of the Plant
Parenthood project. This includes putting together the Raspberry Pi, installation into the plant, and
laying the architecture for the solution – I created and deployed the database, API, Pi, and Android client
and ensured that each endpoint was able to communicate with each-other. I certainly applied and built
upon the foundation of the initial assessment from the Fall, but I feel that much of my learning came
from the unforeseen difficulties and challenges that came from creating this project from the ground up.

More specifically I learned how to create a service (that begins on startup) on a Raspberry Pi,
able to read sensor data and communicate that data with a server utilizing gRPC. That server (the API)
functions as the control layer that communicates with the Azure SQL Database through Entity
Framework, and also feeds data directly to the Android client written in primarily Kotlin. I feel that I’ve
become far more competent in producing functional project architecture – the most difficult part was
just getting everything set up. Once we had the connection wired and gRPC was functioning as expected
the rest followed from prior experience within the Computer Science curriculum. I also feel that I’ve
grown in competency programming in multiple languages (C#, Python, Kotlin, Java), I feel that I’ve
significantly grown in my understanding of real data retrieval and the hardware aspect of computer
engineering, and I have a much better understanding of the client / server relationship.

To be honest, Covid-19 was a major obstacle. There were many parts we weren’t aware that we
needed until we needed them (Analog to Digital Converter, additional wiring, breadboards, soldering),
and at that point shipping moved from 2 days to 3 weeks and our ability to shop freely was significantly
inhibited. We found what we needed, but it was certainly an unforeseen difficulty.