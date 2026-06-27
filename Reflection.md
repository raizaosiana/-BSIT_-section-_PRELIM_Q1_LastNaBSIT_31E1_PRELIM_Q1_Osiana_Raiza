1.Why did you use inheritance?

Inheritance was used to avoid repeating common code and to model the relationship between vehicles. All transport types share common properties such as Name and Capacity, so they inherit these from the Vehicle base class. 
Each specific vehicle such as Car, Boat, or Airplane can then add its own unique behavior while reusing the common features.

2.Why did you use interfaces?

Interfaces were used to define what a vehicle can do rather than what it is. They allow different classes to have the same behaviors without requiring them to share the same parent class.

3.Can Helicopter inherit from both Vehicle and Airplane? Why or why not?

C# does not support multiple inheritance of classes. A class can inherit from only one base class.
Instead, Helicopter should inherit from one class usually Vehicle and implement any interfaces it needs.

4.Why can Helicopter implement both IFlyable and IDriveable?

Because C# allows multiple interfaces. Interfaces only define behaviors, so a class can implement as many interfaces as needed. 
This means the helicopter has both flying and driving-related behaviors without inheriting from multiple classes.

5. If a Submarine can both sail and dive, how would you design it?
I would make the Submarine inherit from Vehicle because it is a type of vehicle. Then, I would implement the ISailable and IDiveable interfaces because a submarine can both sail on the water's surface and dive underwater.
This design keeps the code reusable and flexible.
