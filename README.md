# solana_interview_Qs for Data Scientist position

1. Assume you are flipping a fair coin four times, what is a more likely result (2 heads, 2 tails) or (1 head, 3 tails)?
Flip combinations: (H,H,H,H), (T,H,H,H), (H,T,H,H), (H,H,T,H), (H,H,H,T), (T,T,H,H), (T,H,T,H), (T,H,H,T), (H,T,T,H), (H,T,H,T), (H,H,T,T), (T,T,T,H), (T,T,H,T), (T,H,T,T), (H,T,T,T), (T,T,T,T)
probability of 2 heads and 2 tails = 6/16 = 3/8
probability of 1 head, 3 tails = 4/16 = 1/4
2 heads and 2 tails are more likely

2. You are given an array with [1, 4, '2', '3', 'f', 'sf', 'b', '3', 'b', '4', '2']
 python solution:

ad =[]
source = [1, 4, '2', '3', 'f', 'sf', 'b', '3', 'b', '4', '2']
for i in source:
  if i not in ad:
    ad.append(i)
  elif type(i)=='str':
    if 'b' in i:
      ad.append(i)
