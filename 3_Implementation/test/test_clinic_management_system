
#include "unity.h"
#include <clinic.h>

/* Modify these two lines according to the project */
#include <clinic.h>
#define PROJECT_NAME    "clinic managaement system"

/* Prototypes for all the test functions */
void test_add(void);
void test_read(void);
void test_view(void);
void test_search(void);
void test_edit(void);
void test_delete(void);
void test_show(void);
void test_write(void);
/* Required by the unity test framework */
void setUp(){}
/* Required by the unity test framework */
void tearDown(){}

/* Start of the application test */
int main()
{
/* Initiate the Unity Test Framework */
  UNITY_BEGIN();

/* Run Test functions */
  RUN_TEST(test_add);
  RUN_TEST(test_read);
  RUN_TEST(test_view);
  RUN_TEST(test_edit);
  RUN_TEST(test_search);
  RUN_TEST(test_delete);
  RUN_TEST(test_show);
  RUN_TEST(test_write);
  /* Close the Unity Test Framework */
  return UNITY_END();
}

/* Write all the test functions */ 
void test_add(void) {
    printf("\n\n");
    printf("Already data inputed on the database =%d\n\n",num);//how many inputs
    printf("How many entry do you want to add=\n");
    scanf("%d",&input);
    TEST_ASSERT_EQUAL(sum=input+num);

    for(i=num,j=0; i<sum; i++)
    {
        printf("\n");
        fflush(stdin);
        printf("Enter patient's Name = ");
        TEST_ASSERT_EQUAL(gets(x[i].name));
        fflush(stdin);
        printf("Enter disease = ");
        gets(x[i].disease);
        fflush(stdin);
        printf("Enter the age = ");
        scanf("%d",&x[i].age);
        fflush(stdin);
        printf("Enter cabin no = ");
        scanf("%d",&x[i].cabin);
        fflush(stdin);
        printf("Enter phone number = ");
        scanf("%d",&x[i].phone);
        fflush(stdin);
        printf("\n");
        j++;
        a++;
        num++;
    }
}
void test_delete(void);

{
    int f,h;
    printf("Enter the serial number of the patient that you want to delete=");
    scanf("%d",&f);
    if(f<num)
    {
        printf("What do you want ?\n");
        printf("1.Remove the whole record\n2.Remove Name\n3.Remove Disease\n4.Remove age\
        scanf("%d",&h);
        if(h==1)
        {
            while(f<num)
            {
               TEST_ASSERT_EQUAL(strcpy(x[f].name,x[f+1].name));
               TEST_ASSERT_EQUAL(strcpy(x[f].disease,x[f+1].disease));
               TEST_ASSERT_EQUAL(x[f].age=x[f+1].age);
               TEST_ASSERT_EQUAL(x[f].cabin=x[f+1].cabin);
               TEST_ASSERT_EQUAL(x[f].phone=x[f+1].phone);
                f++;
            }
            num--;
        }
        else if(h==2)
        {
            strcpy(x[f].name,"Cleared");

        }
        else if(h==3)
        {
            strcpy(x[f].disease,"Cleared");
        }
        else if(h==4)
        {
            x[f].age=0;
        }
        else if(h==5)
        {
            x[f].cabin=0;
        }
        else if(h==6)
        {
            x[f].phone=0;
        }

    }
    else
        printf("\n\nInvalid Serial number\n");

}
void test_read(void)
{
    FILE *fp = fopen("patient.txt","r");
    if(fp == NULL)
    {
        TEST_ASSERT_EQUAL(fp = fopen("patient.txt","w"));
        fclose(fp);
        printf("File does not exist, I JUST CREATED IT, exiting...\n\n\n");
        return 0;
    }

   TEST_ASSERT_EQUAL( num = fread(x, sizeof(struct ad),100, fp));
    fclose(fp);
}
void test_void view()
{
    for(i=0; i<num; i++)
    {
        printf("\n");
        printf("Serial Number=%d\n",i);
        printf("Name = ");
        TEST_ASSERT_EQUAL(puts(x[i].name));
        printf("Disease = ");
        TEST_ASSERT_EQUAL(puts(x[i].disease));
        printf("Cabin no = %d\nPhone number = 0%d\nAge=%d",x[i].cabin,x[i].phone,x[i].age);
        printf("\n\n");
    }
}
void test_write(void)
{
    FILE *fp = fopen("patient.txt","w");
    if(fp == NULL)
    {
        printf("Error");
        exit(1);
    }
    TEST_ASSERT_EQUAL(fwrite(x, sizeof(struct ad),num, fp));

    fclose(fp);
}



