import java.util.Scanner;
public class Burc {
    public static void main(String[] args){
        int gün, ay;
        String burc ="";
        boolean isError = false;

        Scanner input = new Scanner(System.in);

        System.out.print("Kaçıncı ayda doğdunuz: ");
        ay =input.nextInt();

        System.out.print("Hangi günde doğdunuz: ");
        gün=input.nextInt();

        switch (ay){
            case 1:
                if (gün>=1&&gün<31){
                    if(gün<21){
                        burc = "OĞLAK";
                    }else {
                        burc = "KOVA";
                    }
                }else{
                    isError= true;
                }
                break;

            case 2:
                if (gün>=1&&gün<29){
                    if(gün<19){
                        burc = "KOVA";
                    }else {
                        burc = "BALIK";
                    }
                }else{
                    isError= true;
                }
                break;

            case 3:
                if (gün>=1&&gün<31){
                    if(gün<20){
                        burc = "BALIK";
                    }else {
                        burc = "KOÇ";
                    }
                }else{
                    isError= true;
                }
                break;

            case 4:
                if (gün>=1&&gün<30){
                    if(gün<20){
                        burc = "KOÇ";
                    }else {
                        burc = "BOĞA";
                    }
                }else{
                    isError= true;
                }
                break;

            case 5:
                if (gün>=1&&gün<31){
                    if(gün<21){
                        burc = "BOĞA";
                    }else {
                        burc = "İKİZLER";
                    }
                }else{
                    isError= true;
                }
                break;

            case 6:
                if (gün>=1&&gün<30){
                    if(gün<22){
                        burc = "İKİZLER";
                    }else {
                        burc = "YENGEÇ";
                    }
                }else{
                    isError= true;
                }
                break;

            case 7:
                if (gün>=1&&gün<31){
                    if(gün<22){
                        burc = "YENGEÇ";
                    }else {
                        burc = "ASLAN";
                    }
                }else{
                    isError= true;
                }
                break;

            case 8:
                if (gün>=1&&gün<31){
                    if(gün<22){
                        burc = "ASLAN";
                    }else {
                        burc = "BAŞAK";
                    }
                }else{
                    isError= true;
                }
                break;

            case 9:
                if (gün>=1&&gün<30){
                    if(gün<22){
                        burc = "BAŞAK";
                    }else {
                        burc = "TERAZİ";
                    }
                }else{
                    isError= true;
                }
                break;

            case 10:
                if (gün>=1&&gün<31){
                    if(gün<22){
                        burc = "TERAZİ";
                    }else {
                        burc = "AKREP";
                    }
                }else{
                    isError= true;
                }
                break;

            case 11:
                if (gün>=1&&gün<30){
                    if(gün<21){
                        burc = "AKREP";
                    }else {
                        burc = "YAY";
                    }
                }else{
                    isError= true;
                }
                break;

            case 12:
                if (gün>=1&&gün<31){
                    if(gün<21){
                        burc = "YAY";
                    }else {
                        burc = "OĞLAK";
                    }
                }else{
                    isError= true;
                }
                break;

        }
        if(isError){
            System.out.println("Geçersiz bir gün girdiniz...");

        }else {
            System.out.println("Burcunuz: "+ burc);
        }


    }
}
