public class EarphoneExample {
    public static void main(String args[]) {
        System.out.println("The main class");
        Earpod EarpodObj = new Earpod();
        EarpodObj.Connect(400f, 2.5f);

    } 
    
}
class Earphone{

}
class Earpod extends Earphone //isA
{
    private Bluetooth Bluetoothobj = new Bluetooth();// hasA
    void Connect(float range, float frequency )//useA
    {
        
        if(range<=300 || frequency >=2.4 ){
            System.out.println("the device is connected and audio is produce");
            
        }
        else{
            System.out.println(" searching for the device ");
        }
    }

}
class Technology{

}
class Bluetooth extends Technology// isA
{

}
