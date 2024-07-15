# leetcode_coding_problem_solutions
<h5> problem code FIT </h5>
Chef wants to become fit for which he decided to walk to the office and return home by walking. It is known that Chef's office is X km away from his home.
If his office is open on 5 days in a week, find the number of kilometers Chef travels through office trips in a week.
# Solution
![image](https://user-images.githubusercontent.com/97357575/175786762-53f4bbb2-f849-4e63-ac90-4429bf2a055c.png)

<h5> problem code DNASTRAND </h5>
You are given the sequence of Nucleotides of one strand of DNA through a string S of length N. S contains the character A,T,C, and G only.

Chef knows that:

A is complementary to T.
T is complementary to A.
C is complementary to G.
G is complementary to C.
Using the string S, determine the sequence of the complementary strand of the DNA.

# Solution
#include <iostream>
using namespace std;

int main() {
	// your code goes here
	int t,n;
	cin>>t;
	while(t!=0)
	{
	 cout << endl;
	 cin>>n;
	 char s[n];
	 char out[n];
	 for(int i=0;i<n;i++)
	 {
	    
	     cin>>s[i];
	    
	         if(s[i]=='A')
	         {
	             s[i]='T';
	            
	         }
	        else if(s[i]=='T')
	         {
	             s[i]='A';
	            
	         }
	         else if(s[i]=='C')
	         {
	             s[i]='G';

	         }
	         else if(s[i]=='G')
	         {
	             s[i]='C';

	         }
	          out[i]=s[i];
	    
	    
	 }
	 for(int i=0;i<n;i++)
	 {
	     cout<<out[i];
	 }
	 t--;
	}

	return 0;
}



