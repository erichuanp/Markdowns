# 2.1 Negations

**Description**: If P has a truth value. The *negation* of P is *not P's truth value*. 

### **Example**

P = True
not P = False

### **Summary**

You firstly exchange the conjunction $\cap$ and $\cup$, then make each substatement as negative.

> P$\cap$Q = (!P)$\cup$(!Q)

### **Example**

I made it right and the answer equals three. I didn't make it right or the answer doesn't equal three. 

# 2.3 If then

**Description**: We cannot have P without Q. (Not P) $\cup$ Q. 

### **Example**

P: A drinks water. **Requirement.** 

Q: A dies. **Result.** 

P$\Rightarrow$Q: If A drinks water, then A dies. 

| P   | Q   | P$\Rightarrow$Q | (not P)$\cup$Q | Description                                                             |
|:---:|:---:|:---------------:|:--------------:|:----------------------------------------------------------------------- |
| T   | T   | T               | T              | Eric drank water then Eric died. So the statement is true.              |
| T   | F   | F               | F              | Eric drank water, but Eric didn't die. So the statement is false.       |
| F   | T   | T               | T              | Eric didn't drink water but Eric died. So the statement is true.        |
| F   | F   | T               | T              | Eric didn't drink water then Eric didn't die. So the statement is true. |

### **Summary**

Most of the time it depends on Q's truth value. If Q is T then P$\Rightarrow$Q is T. If Q is F and P is F too, then P$\Rightarrow$Q is true. 

### Negation

**Description**: not (P$\Rightarrow$Q) == P $\cap$ (not Q)

### **Example**

P: the crust is brown\
Q: the pie is done.\
Negation: The crust is brown, and the pie is not done. **(Make P$\Rightarrow$Q to false)**

P: it is raining, and I have to leave the house\
Q: I take an umbrella\
Negation: It is raining, and I have to leave the house, and I am not taking an umbrella.

## 2.3.1 Converse and Contrapositive

**Definition**: The *converse* of P$\Rightarrow$Q is the statement Q$\Rightarrow$P. The *contrapositive* of P$\Rightarrow$Q is the statement (not Q)$\Rightarrow$(not P).

### **Example**

P: raining Q: street gets wet\
*Converse*: If street gets wet, then raining.\
*Contrapositive*: If street doesn't get wet, then it's not raining. 