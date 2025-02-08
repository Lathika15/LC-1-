#include <stdio.h>
#include <stdlib.h>
struct node{
    int n;
    struct node* next;
    
};


void reverse(struct node *h){
    struct node *temp,*prev,*p,*ne;
    temp=h;
    
    p=h->next;
             int count=0;
    while(p!=NULL  && count!=10){
        prev=temp;
        ne=h->next;

        while(ne->next!=NULL && count!=10)
        {
              //printf("%d ",ne->n);
            prev=ne;
            ne=ne->next;
            count++;
        }
       // printf("ne over\n");
        prev->next=NULL;
        temp->next=ne;
      
        ne->next=p;
        temp=temp->next;
        printf("%d ",ne->n);
    }
}
void display(struct node *h) {
    struct node *t = h->next;
    if (t != NULL) {
        while (t != NULL) {
            printf("%d ", t->n);
            t = t->next;
        }
    } else {
        printf("List is empty.\n");
    }
    printf("\n");
}

   
void insert(int data,struct node *h){
    struct node* new=(struct node *)malloc(sizeof(struct node));
    new->n=data;
    new->next=h->next;
    h->next=new;
}
int main()
{
    struct node *h;
    h=(struct node *)malloc(sizeof(struct node));
    h->next=NULL;
    insert(1,h);
    insert(2,h);
    insert(3,h);
    insert(4,h);
    display(h);
    reverse(h);
    display(h);
    return 0;
}
