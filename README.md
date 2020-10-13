# HelloWorld
//1、给定数组int[] arr = new int[] { 100, 60, 20, 30, 20, 10, 50, 60, 90 ,40};
//要求：将该数组元素存储集合，并实现：去除重复并排序

package test;
public static void main(String[] args) {

		int[] arr = new int[] { 100, 60, 20, 30, 20, 10, 50, 60, 90 ,40};
		Set<Integer> set = new HashSet<>();
		for (int i = 0; i < arr.length; i++) {
			set.add(arr[i]);
		}
		List<Integer> list = new ArrayList<>();
		for (int i : set) {
			list.add(i);
		}
		Collections.sort(list);
		System.out.println(list);
	}
