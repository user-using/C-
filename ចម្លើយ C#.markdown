# ចម្លើយសំណួរអំពី C# Programming សម្រាប់ Desktop Application

1. **ថាតើ class ជាអ្វី? មានប្រភេទ class អ្វីខ្លះ? គោលបំណងរបស់វាជាអ្វី?**  
class ក្នុង C# គឺជាផែនការសម្រាប់បង្កើត objects ដោយកំណត់ properties, methods, និង behavior។  
ប្រភេទ class:  
- **Concrete class**: class ធម្មតាដែលអាច instantiate បាន (ឧ. class Car {}).  
- **Abstract class**: មិនអាច instantiate បាន; ប្រើជា base class (ឧ. abstract class Vehicle {}).  
- **Sealed class**: មិនអាច inherit បាន (ឧ. sealed class FinalClass {}).  
- **Static class**: មានតែ static members; មិនអាច instantiate បាន (ឧ. static class Utility {}).  
គោលបំណង: រៀបចំ code អនុញ្ញាត object-oriented programming (OOP) និងគាំទ្រ inheritance, encapsulation, និង polymorphism។

2. **ថាតើ Constructor ជាអ្វី?**  
Constructor គឺជា method ពិសេសក្នុង class ដែលមានឈ្មោះដូច class ប្រើដើម្បី initialize objects។ វាត្រូវបានហៅនៅពេលបង្កើត object ដោយប្រើ keyword new (ឧ. Car() {} ក្នុង class Car)។

3. **ថាតើ inheritance ជាអ្វី?**  
inheritance អនុញ្ញាតឱ្យ class (derived/child) ទទួល properties និង methods ពី class ផ្សេង (base/parent)។ វាលើកកម្ពស់ការប្រើប្រាស់ code ឡើងវិញ (ឧ. class Sedan : Car {} inherits ពី Car)។

4. **ថាតើ virtual members ជាអ្វី?**  
virtual members គឺជា methods, properties, ឬ events ក្នុង base class ដែលអាច override ក្នុង derived class។ ផ្លាកដោយ keyword virtual (ឧ. public virtual void Drive() {}) ដែលអនុញ្ញាតឱ្យមាន polymorphism។

5. **ថាតើ abstract method ជាអ្វី?**  
abstract method គឺជា method ក្នុង abstract class ដែលគ្មាន implementation ផ្លាកដោយ keyword abstract។ derived classes ត្រូវ override (ឧ. public abstract void Start();)។

6. **ថាតើ Default constructor ជាអ្វី? class តែងតែមាន Default constructor ឬអត์?**  
Default constructor គឺជា constructor ដែលគ្មាន parameters ដែល C# ផ្តល់ដោយស្វ័យប្រវត្តិប្រសិនបើគ្មាន constructors ត្រូវបានកំណត់ (ឧ. public ClassName() {})។ ប្រសិនបើអ្នកកំណត់ constructor ណាមួយ Default constructor នឹងមិនត្រូវបានផ្តល់ទេ។

7. **ថាតើ encapsulation ជាអ្វី?**  
encapsulation គឺជាគោលការណ៍ OOP នៃការបញ្ចូល data (fields) និង methods ដែល operate លើ data នោះក្នុង class មួយ ជាញឹកញាប់ប្រើ access modifiers ដូចជា private, public, ឬ protected ដើម្បីគ្រប់គ្រង access (ឧ. ប្រើ private int speed; ជាមួយ public getter/setter)។

8. **ថាតើ static members ជាអ្វី?**  
static members ជាកម្មសិទ្ធិរបស់ class ផ្ទាល់ មិនមែន instance និងត្រូវបាន share ក្នុងចំណោម objects ទាំងអស់។ ផ្លាកដោយ keyword static (ឧ. public static int Count;)។ វាមានប្រយោជន៍សម្រាប់ shared data ឬ utility methods។

9. **ថាតើ static constructor ជាអ្វី?**  
static constructor គឺជា constructor ដែល initialize static members នៃ class។ វាគ្មាន parameters ផ្លាកដោយ static និងត្រូវបានហៅដោយស្វ័យប្រវត្តិមុនពេល instance ដំបូងត្រូវបានបង្កើត ឬ static members ណាមួយត្រូវបាន access (ឧ. static ClassName() {})។

10. **ថាតើ keyword protected ជាអ្វី?**  
keyword protected គឺជា access modifier ដែលអនុញ្ញាត access ទៅ member ក្នុង class ដូចគ្នា ឬ derived classes (ឧ. protected int speed; អាច access ដោយ subclass)។

11. **ថាតើ C# properties ជាអ្វី? ហេតុអ្វីបានជាប្រើវាជំនួស fields?**  
properties ផ្តល់នូវវិធី controlled ដើម្បី access private fields ដោយប្រើ get និង set accessors (ឧ. public int Speed { get; set; })�। វាត្រូវបានប្រើជំនួស fields សម្រាប់ encapsulation, validation, ឬ computed values (ឧ. get { return speed * 2; })។

12. **inheritance អនុញ្ញាតឱ្យ derived classes access data ក្នុង base class យ៉ាងដូចម្តេច?**  
inheritance អនុញ្ញាតឱ្យ derived class access public, protected, និង internal members នៃ base class។ private members មិនអាច access បានទេ លើកលែងតែ exposed តាម properties ឬ methods (ឧ. base.SomeMethod() calls base class method)។

13. **ថាតើ sealed class ជាអ្វី?**  
sealed class មិនអាច inherit បានទេ។ ផ្លាកដោយ keyword sealed (ឧ. sealed class FinalClass {})។ ប្រើដើម្បី prevent ការ inheritance បន្ថែមសម្រាប់ security ឬ design reasons។

14. **ថាតើ overloading method ជាអ្វី?**  
method overloading អនុញ្ញាតឱ្យមាន methods ជាច្រើនដែលមានឈ្មោះដូចគ្នា ប៉ុន្តែ parameter lists ផ្សេងគ្នា (ឧ. void Print(int x) និង void Print(string x))។ វា enhances flexibility ក្នុង method usage។

15. **ថាតើ overriding method ជាអ្វី?**  
method overriding អនុញ្ញាតឱ្យ derived class ផ្តល់ specific implementation នៃ virtual ឬ abstract method ពី base class ដោយប្រើ keyword override (ឧ. public override void Drive() {})។

ប្រសិនបើអ្នកត្រូវការការពន្យល់បន្ថែម សូមប្រាប់ខ្ញុំ!