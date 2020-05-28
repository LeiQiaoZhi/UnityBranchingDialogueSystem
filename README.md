# Branching Dialogue System for Unity
A **node based** branching dialogue system created by me for Unity,  which can visualise the dialogues in **graphs**. 

 <img src="https://github.com/LeiQiaoZhi/UnityBranchingDialogueSystem/blob/master/Screenshot%202020-05-28%2020.03.38.png" alt="Italian Trulli">
 
*warning -- the graph's current capabilities are limited. It is mostly for visualisation of already created dialogue nodes. Text and connections between existing nodes can be edited and saved. However, new nodes cannot be created in the graph, yet.*


## Structure
two custom scriptable objects are created for dialogues, which are dialogue and sentence

### Dialogue
A dialogue is basicly the first sentence of a dialogue. By choosing a dialogue scriptable object, the dialogue manager or the graph editor window knows the flow of the entire dialogue as each sentence is chained to another.
It also has a public bool variable called is available. The dialogue 

### Sentence
A sentence is the building block of dialogues. Each sentence sciptable object has several fields.
#### From(StringVariable)
a string variable representing the name of the speaker.(I am using a sciptable object named StringVariable to store the character name data, I will get to that later)
#### Text(string)
The actual text of the sentence.
### Next Sentence(Sentence)
The next sentence. 
### Options(List<Choice>)
A resizeable list of choices. If a sentence has choices, the Text and Next Sentence 
 
<img src="https://github.com/LeiQiaoZhi/UnityBranchingDialogueSystem/blob/master/Screenshot%202020-05-28%2022.59.49.png" alt="Italian Trulli" width="30%" height="30%">
 <img src="https://github.com/LeiQiaoZhi/UnityBranchingDialogueSystem/blob/master/Screenshot%202020-05-28%2023.00.09.png" alt="Italian Trulli" width="30%" height="30%">



