### [Breaking the Records](https://www.hackerrank.com/challenges/three-month-preparation-kit-breaking-best-and-worst-records/problem?isFullScreen=true&h_l=interview&playlist_slugs%5B%5D=preparation-kits&playlist_slugs%5B%5D=three-month-preparation-kit&playlist_slugs%5B%5D=three-month-week-one)
##### Description
      Input : 3 4 21 36 10 28 35 5 24 42
      Output : 4 0
      Hint: click on the above link to read problem statement.
#### Solution:

```csharp
class Result
{
    public static List<int> breakingRecords(List<int> scores)
    {
        int min=0,mincount=0,max=0,maxcount=0;
        min=max=scores[0];
        for(int i=1;i<scores.Count;i++){
            if(scores[i] <  min){
                min=scores[i];
                mincount++;
            }
            if(scores[i] > max){
                max=scores[i];
                maxcount++;
            }
        }
        return new List<int>(){maxcount,mincount};
    }   
}
```
