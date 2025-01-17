### Sonali Patel - 40176580

## Basic Calculator

Step 1: Control Flow Graph for onClick(): <br/>
<img height="300" alt="Calculator CFG" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-sonalipxtel/assets/141271290/3186633d-f66a-4f68-9740-bf73a22f6568">
<br/><br/>

Step 2: Node Coverage <br/>
TR: [1], [2], [3], [4], [5], [6], [7], [8], [9], [10], [11], [12], [13], [14], [15], [16], [17], [18], [19], [20], [21], [22], [23] <br/>
Test Path: [1,2,23], [1,3,23], [1,4,23], [1,5,23], [1,6,23], [1,7,23], [1,8,23], [1,9,23], [1,10,23], [1,11,23], [1,12,23], [1,13,23], [1,14,23], [1,15,23], [1,16,17,18,22,23], [1,16,17,19,22,23], [1,16,17,20,22,23], [1,16,17,21,22,23] <br/>

Step 3: Edge Coverage <br/>
TR: [1,2], [1,3], [1,4], [1,5], [1,6], [1,7], [1,8], [1,9], [1,10], [1,11], [1,12], [1,13], [1,14], [1,15], [1,16], [2,23], [3,23], [4,23], [5,23], [6,23], [7,23], [8,23], [9,23], [10,23], [11,23], [12,23], [13,23], [14,23], [15,23], [16,17], [17,18], [17,19], [17,20], [17,21], [18,22], [19,22], [20,22], [21,22], [22,23]<br/>
Test Path: [1,2,23], [1,3,23], [1,4,23], [1,5,23], [1,6,23], [1,7,23], [1,8,23], [1,9,23], [1,10,23], [1,11,23], [1,12,23], [1,13,23], [1,14,23], [1,15,23], [1,16,17,18,22,23], [1,16,17,19,22,23], [1,16,17,20,22,23], [1,16,17,21,22,23] <br/>

Step 4: Edge-Pair Coverage <br/>
TR: [1,2,23], [1,3,23], [1,4,23], [1,5,23], [1,6,23], [1,7,23], [1,8,23], [1,9,23], [1,10,23], [1,11,23], [1,12,23], [1,13,23], [1,14,23], [1,15,23], [1,16,17], [16,17,18], [16,17,19], [16,17,20], [16,17,21], [18,22,23], [19,22,23], [20,22,23], [21,22,23] <br/>
Test Path: [1,2,23], [1,3,23], [1,4,23], [1,5,23], [1,6,23], [1,7,23], [1,8,23], [1,9,23], [1,10,23], [1,11,23], [1,12,23], [1,13,23], [1,14,23], [1,15,23], [1,16,17,18,22,23], [1,16,17,19,22,23], [1,16,17,20,22,23], [1,16,17,21,22,23] <br/>

Step 5: Event Flow Graph for Basic Calculator: <br/>
<img width="300" alt="Calculator EFG" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-sonalipxtel/assets/141271290/f3bf56c3-466f-4dba-9877-4a20b242b324">
<br/><br/>

Step 6: Monkey Runner

## Lexica App
I selected the wordListToString() method that converts a list of words into a single string:
```
    private String wordListToString() {
        StringBuilder sb = new StringBuilder();
        ListIterator<String> li = wordList.listIterator();

        while (li.hasNext()) {
            String w = li.next();
            sb.append(w);
            if (li.hasNext()) {
                sb.append(",");
            }
        }
        return sb.toString();
    }
```
Step 1: Control Flow Graph for wordListToString(): <br/>
<img width="300" alt="Lexica CFG" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-sonalipxtel/assets/141271290/65cc7e22-5616-486b-ba0a-55dbcb601e1e">
<br/><br/>

Step 2: Node Coverage <br/>
TR: [1], [2], [3], [4], [5], [6] <br/>
Test Path: [1,2,3,4,5,2,6] <br/>

Step 3: Edge Coverage <br/>
TR: [1,2], [2,3], [3,4], [4,5], [5,2], [2,6] <br/>
Test Path: [1,2,3,4,5,2,6] <br/>

Step 4: Edge-Pair Coverage <br/>
TR: [1,2,3], [2,3,4], [3,4,5], [4,5,2], [5,2,6], [1,2,6] <br/>
Test Paths: [1,2,6], [1,2,3,4,5,2,6] <br/>

Step: Event Flow Graph for Lexica <br/>
<img height="300" alt="Lexica EFG" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-sonalipxtel/assets/141271290/fe4fff7c-36fc-4473-84ec-dcc38a5081dc">
<br/><br/>


