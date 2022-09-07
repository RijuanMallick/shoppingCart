#include <bits/stdc++.h>
using namespace std;

int main()
{
    // pair<string,pair<int,int>> product;
    struct product{
        string name;
        int price;
        int gst;
        int quantity;
    };
    vector<product> curt;
    product p1;
    p1.name="Leather wallet";
    p1.price=1100;
    p1.gst=18;
    p1.quantity=1;
    product p2;
    p2.name="Umbrella";
    p2.price=900;
    p2.gst=12;
    p2.quantity=2;
    product p3;
    p3.name="Cigarette";
    p3.price=200;
    p3.gst=28;
    p3.quantity=3;
    product p4;
    p4.name="Honey";
    p4.price=100;
    p4.gst=0;
    p4.quantity=4;
    
    curt.push_back(p1);
    curt.push_back(p2);
    curt.push_back(p3);
    curt.push_back(p4);
    pair<string,int> max_gst;
    max_gst={" ",0};
    int total_price=0;
    int total_discunt=0;
    for(int i=0;i<curt.size();i++){
        product p=curt[i];
        total_price=total_price+(p.price*p.quantity)+(p.price*p.quantity*p.gst/100);
        if(p.price>500){
            int x=(p.price*p.quantity)+(p.price*p.quantity*p.gst/100);
            total_discunt=total_discunt+(x*5/100);
        }
        int y=(p.price*p.quantity*p.gst/100);
        if(max_gst.second<y){
            max_gst.first=p.name;
            max_gst.second=y;
        }
        
    }
    cout<<"Total Amount -->"<<total_price<<endl;
    cout<<"Total Discunt -->"<<total_discunt<<endl;
    cout<<"Total Amount To Be Paid -->"<<total_price-total_discunt<<endl;
    cout<<"The product for Which You Paid Max GST -->"<<max_gst.first;
    
    return 0;
}
