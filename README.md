# reverse_eachword

package elclipse;

public class reverse_eachword {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		String s="Harsh is the best coder";
		String output="";
		int index=0;
		for(int i=0;i<s.length();i++) {
			if(s.charAt(i)==' ') {
				index=i+1;
				output+=s.charAt(i);
			}
			else {
				output=output.substring(0,index) +s.charAt(i) + output.substring(index);
			}
		}
		System.out.print(output);
	}

}


///////time complexity is O(N)
