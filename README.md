# Module3
Data.frame

Assignment # 3

The data set below is based on the presidential election during 2016, where it outlined the name of the candidate, the source of the poll (ABC vs, CBS). Discuss your result in your blog. Important note, I made up this data, so this data does not reflect what really happened in the election.

> Name <- c("Jeb", “Donald”, "Ted”, “Marco” “Carly”, “Hillary”, “Berine”)

> ABC political poll results <- c(4, 62 51, 21, 2, 14, 15)

> CBS political poll results <- c(12, 75, 43, 19, 1, 21, 19) 

Your assignment is how do you convert the two data containers (ABC and NCB) into data.frame? and how do you calculate the mean in this data.frame?



> Name <- c("Jeb", "Donald", "Ted", "Marco", "Carly", "Hillary", "Bernie")

> ABC_Political <- c(4,62,51,21,2,14,15)

> CBS_Political <- c(12,75,43,19,1,21,19)

> results <- cbind(Name, ABC_Political, CBS_Political)

> results

     Name      ABC_Political CBS_Political

[1,] "Jeb"     "4"           "12"         

[2,] "Donald"  "62"          "75"         

[3,] "Ted"     "51"          "43"         

[4,] "Marco"   "21"          "19"         

[5,] "Carly"   "2"           "1"          

[6,] "Hillary" "14"          "21"         

[7,] "Bernie"  "15"          "19"         

> results.df=data.frame(Name, ABC_Political, CBS_Political)

> results.df

     Name ABC_Political CBS_Political

1     Jeb             4            12

2  Donald            62            75

3     Ted            51            43

4   Marco            21            19

5   Carly             2             1

6 Hillary            14            21

7  Bernie            15            19

> r=rowMeans(results.df[,2:3])

> r.df=data.frame(Name,r)

> mean(as.matrix(results.df[,2:3]))

[1] 25.64286

