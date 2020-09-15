1.帮助开发人员编写代码，提升质量、减少bug。
2.提升反馈速度，减少重复工作，提高开发效率。
3.保证你最后的代码修改不会破坏之前代码的功能。
4.让代码维护更容易。5.有助于改进代码质量和设计。
public class Test9 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int score[] = {25, 24, 12, 76, 101, 96,28};
		bubbleArray(score);
		printArray(score);
	}
	public static void printArray(int score[]) {
		for(int i = 0; i < score.length; i++) {
			 System.out.print(score[i] +" ");
		}
		System.out.println();
	}
	private static void bubbleArray(int[] score) {
		for(int i = 0;i < score.length - 1;i ++) {
			for(int j = 0;j < score.length - i -1; j++) {
				if(score[j] > score[j + 1]) {
					int temp = score[j];
					score[j] = score[j + 1];
					score[j + 1] = temp;
				}
			}
		}
	}
}
