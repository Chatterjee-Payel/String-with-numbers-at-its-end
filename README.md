# String-with-numbers-at-its-end
class Solution{
public:	
		
		
	int isSame(string s)
	{
	   int count=0,num=0;
	   for(int i=0;i<s.size();i++){
	       if(s[i]>='a' && s[i]<='z'){
	           count++;
	       }
	       else{
	           num=num*10+(s[i]-'0');
	       }
	       
	   }
	   if(count==num)
	   {
	       return 1;
	   }
	   return 0;
	}
};
