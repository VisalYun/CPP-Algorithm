Given a square matrix, calculate the absolute difference between the sums of its diagonals.

For example, the square matrix arr is shown below:
```
1 2 3
4 5 6
9 8 9 
```
The left-to-right diagonal = 1 + 5 + 9 = 15. The right to left diagonal = 3 + 5 + 9 = 17. Their absolute difference is |15 - 17| = 2.

**Spoiler**: This is the solution:
```
int diagonalDifference(vector<vector<int>> arr) 
{
    int n=arr.size(),diag=0,antidiag=0,sum=0,i;
    for(i=0;i<n;i++)
    {
        diag+=arr[i][i];
        antidiag+=arr[i][(n-1)-i];
    }
    sum=abs(diag-antidiag);
    return sum;
}
```