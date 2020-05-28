# UnityBranchingDialogueSystem
A **node based** branching dialogue system created by me for Unity,  which can visualise the dialogues in **graphs**. 

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
### Next Sentence
