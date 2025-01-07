# Lecture 1 (1/6/25)

## Things I'm confused about 
### how to calculate big O 

## After class TODO
- 

## Things I'm confused about 


## Notes
### BIG O 
for(i = n; i >= 1; i /= 2)
  for(j = 1; j<= 5i; j++)
    x++;
- assume n = 2^k
- count how many times the loop will go for
  - when i = 2^k, j= 1, 2, 3, 4, 5x2^k
  - when i = 2^(k-1), j= 1, 2, 3, 4, 5x2^(k-1)
  - when i = 2^(k-2), j= 1, 2, 3, 4, 5x2^(k-2)
  - when i = 2^(k-k), j= 1, 2, 3, 4, 5x1
- comees out as geometric summation  
  <img width="1324" alt="Screenshot 2025-01-06 at 19 28 28" src="https://github.com/user-attachments/assets/b13d986e-259b-4661-bf72-2c1e8575b5da" />  <br/>
 
### Pre/IN/Post order
  a<br/>
/   |<br/>
b     c

- pre -> a, b, c
- in -> b, a, c
- post -> b, c, a

## Terms/Vocabs/ect.
- 
