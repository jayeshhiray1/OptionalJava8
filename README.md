# OptionalJava8
Optional is a container object used to contain not-null objects. Optional object is used to represent null with absent value. This class has various utility methods to facilitate code to handle values as ‘available’ or ‘not available’ instead of checking null values. It is introduced in Java 8 and is similar to what Optional is in Guava.


![image](https://user-images.githubusercontent.com/47211382/125505279-4ad2160d-57cc-482f-8f28-8bae9b8e845a.png)

![image](https://user-images.githubusercontent.com/47211382/125505460-1971a31b-b0f7-4aaa-bb8d-064248839a96.png)


##working code

package com.example;

import java.util.Optional;

public class OptionalMethodInjava {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		// Old WAY BEFORE JAVA 8
//		String str = "Values is there";
//
//		if (str == null) {
//			System.out.println("value is null");
//		} else {
//			System.out.println(str);
//		}

		// After BEFORE JAVA 8
		String str = "Values is there";
		Optional<String> optional = Optional.of(str);

		System.out.println(optional.get());
		System.out.println("isEmpty()--" + optional.isEmpty());
		System.out.println("isPresent()--" + optional.isPresent());
		
		System.out.println("orElse--" + optional.orElse("No values Found"));

	}

}

##Output

Screenshot<img width="626" alt="Screenshot 2021-07-13 at 11 57 19 PM" src="https://user-images.githubusercontent.com/47211382/125505601-2a1013f8-c0d0-43cf-baa4-b9336c79c9e7.png"> 


