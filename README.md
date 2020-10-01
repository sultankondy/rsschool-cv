1. First Name: Sultan
2. Last Name: Kondybay
3. Contact Info:
	- Phone: 87025915772;
	- Email: sltnkondy@gmail.com;
	- Telegram: @sltnkondy;


-----

## Summary:

At the moment I am studying at the university, and my profession is an information system. Now I want a lot in my life, but since I'm a programmer 
I want to learn a lot of programming languages. In general, I know java and I think javascript will not be difficult for me. if I learn good code 
I can work on specialty. and I have big goals and I want to start small from the first.

## Code examples:
```
import java.util.Random;
import java.util.Arrays;
import java.util.Scanner;

public class Dublicate{
	int n;
	Random rand;
	int[] arr;

	public Dublicate(int n){
		arr = new int[n+2];
		rand = new Random();
	} 

	public int[] taskArr(int n){
		int a = rand.nextInt(n);
		for (int i = 0;i<n + 1;i++){
			arr[i] = i; 
		}
		arr[arr.length-1] = a;
		Arrays.sort(arr);
		return arr;
	}

	public int searchDubNum(){
		boolean toggle = true;
		int start = 0;
		int end = arr.length-1;
		int mid = 0;
		while(toggle){
			mid = (start + end)/2;
			if(mid!=arr[mid]){
				end = mid - 1;
			}
			else if(mid==start)
				toggle = false;
			else{
				start = mid;	
			}
			
		}
		return arr[mid + 1];
	}

	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);
		int size = in.nextInt();
		Dublicate dub = new Dublicate(size);
		System.out.println(Arrays.toString(dub.taskArr(size)));
		System.out.println(dub.searchDubNum());
		
	}
}
```

## English:

since I study at the SDU, we have lessons in English and have a good experience in understanding the language
