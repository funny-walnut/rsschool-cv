Valeriya Zinoveva
=================
![photo](rsschool-cv\img\c4lEcs848yQ.jpg)
# Contacts #
* address: Erevan, Armenia
* phone: +374 95219775
* email: leraiztlt@gmail.com
* github: [funny-walnut](https://github.com/funny-walnut)

---
# About myself #
I started learning the frontend 1 month ago. Before that, I worked as QA enjineer at Optimax Dev for 10 months.

---
# Skills #
* HTML 
* CSS
* Git
* Jira
* Basic C#, Java, JavaScript
* PHP
* Codeception
---
# Courses #
[Optimax Dev academy of automation testing](https://optimax.dev/academy/)

---
# Code example #
```java
import java.util.*;

public class Level1
  {
    public static int ConquestCampaign( int N, int M, int L, int [] battalion)
        {
            int [][] field = new int[N][M];

            int day;
            for (int i =0; i<L*2; )
            {
                int a = battalion[i];
                int b = battalion[i+1];
                    field[a-1][b-1]=1;
                    i += 2;
            }
            
                for ( day = 1; day < N*M; day++) {
                    int counter;
                    counter =0;
                    for (int k = 0; k < N; k++) {

                        for (int l = 0; l < M; l++) {
                            if ((field[k][l]) ==0)
                                counter += 1;
                            //System.out.println("counter" + counter);
                        }
                    }
                    if (counter > 0) {

                        for (int i = 0; i < N; i++) //заполняем прилегающие территории
                        {
                            for (int j = 0; j < M; j++) {
                                if (field[i][j] == day) {
                                    if (i + 1 < N && field[i + 1][j]!= day)
                                        field[i + 1][j] = day + 1;
                                    if (j + 1 < M && field[i][j + 1] != day)
                                        field[i][j + 1] = day + 1;
                                    if (i - 1 >= 0 && field[i - 1][j] != day)
                                        field[i - 1][j] = day + 1;
                                    if (j - 1 >= 0 && field[i][j - 1] != day)
                                        field[i][j - 1] = day + 1;
                                }
                            }
                        }
                        
                    } else
                            break;
                }
            return day;
        }
    }
```
# Languages #
* English - (B1)
* Russian - native
