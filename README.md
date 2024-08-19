# REFramework Practical Example - COVID Data Processor

This solution consists of a performer, a dispatcher and a custom developed Power App that acts as a data capturing system.

## Dispatcher Architecture:
The flowchart illustrates a Dispatcher Process that automates the retrieval and filtering of datasets. It begins by opening a web browser and navigating to the Data.World website, where it searches for a specific dataset. Once the dataset is found, it is downloaded for further processing. The downloaded dataset is then filtered to focus on records related to South Africa. These filtered records are subsequently added to a queue, possibly for further processing in a larger automation workflow. The process concludes once the records have been successfully queued. This automation streamlines data extraction and preparation, ensuring relevant information is efficiently gathered and organised. 
![Dispatcher](https://github.com/user-attachments/assets/29ddf7e0-b92f-4b62-898e-2d91bd21f991)
In the context of Robotic Process Automation (RPA), a Dispatcher is a process or bot that primarily focuses on preparing and organising data for further processing. It typically involves tasks such as collecting, filtering, and queuing data. The Dispatcher’s role is to gather the necessary information, often from external sources like websites or databases, and then structure it in a way that can be efficiently handled by subsequent processes, such as a Performer.

## Performer Architecture:
The flowchart represents a Performer Process, a common component in Robotic Process Automation (RPA) that executes tasks based on data received from a Dispatcher Process. The process starts by retrieving items from a queue, which likely contains the filtered data prepared by the Dispatcher. It then initialises the environment by opening the necessary application. Next, the process captures the relevant details from the queued items and submits these details, possibly into another system or database. Finally, the process cleans up the environment, ensuring no residual data or open applications remain, before concluding. The Performer Process is crucial in an RPA workflow as it carries out the detailed tasks that transform data into actionable outcomes.
![Performer](https://github.com/user-attachments/assets/45d008a5-1f33-420a-ab34-617fcaa7bf3e)
