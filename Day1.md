Day-1

Solving Goldman Sachs Question sheet

Q1:-https://www.google.com/url?q=https://practice.geeksforgeeks.org/problems/print-anagrams-together/1/&sa=D&source=editors&ust=1645599845832875&usg=AOvVaw2xS6hdqZbt6ny5kyaknmNH

My Solution:-
class Solution {
    public List<List<String>> Anagrams(String[] string_list) {
        // Code here
        Map<Map<Character,Integer>,List<String>> m=new LinkedHashMap<>();
        for(String i:string_list){
            int sumOfChar=0;
            Map<Character,Integer> t=new TreeMap<>();
            for(int j=0;j<i.length();j++){
                char val=i.charAt(j);
                if(t.containsKey(val)==true){
                    t.put(val,t.get(val)+1);
                }
                else{
                    t.put(val,1);
                }
                // t.put(i.charAt(j),t.get(i.charAt(j))==null?1:t.get(charAt(j))+1);
            }
            List<String> l=new ArrayList<>();
            l.add(i);
            if(m.get(t)!=null){
                List<String> k=new ArrayList<>();
                k.addAll(m.get(t));
                k.addAll(l);
                m.put(t,k);
            }
            else{
               m.put(t,l); 
            }
        }
        List<List<String>> ans=new ArrayList<>();
        for(Map.Entry<Map<Character,Integer>,List<String>> i:m.entrySet()){
            ans.add(i.getValue());
        }
        return ans;
    }
}

Q2-https://www.google.com/url?q=https://practice.geeksforgeeks.org/problems/overlapping-rectangles1924/1/&sa=D&source=editors&ust=1645599845833391&usg=AOvVaw3LxEsRDb2hy19JWwB6CXYu

My Solution:-


Q3:-https://www.google.com/url?q=https://practice.geeksforgeeks.org/problems/count-the-subarrays-having-product-less-than-k1708/1/&sa=D&source=editors&ust=1645599845833855&usg=AOvVaw1ekANCXu_w01gJBkmIfkwT

My Solution:-

Q4:-https://www.google.com/url?q=https://practice.geeksforgeeks.org/problems/run-length-encoding/1/&sa=D&source=editors&ust=1645599845834245&usg=AOvVaw2c7Bs0kcw41LzdbQ8sVDlq

My Solution:-

Q5:-https://www.google.com/url?q=https://practice.geeksforgeeks.org/problems/ugly-numbers2254/1/&sa=D&source=editors&ust=1645599845834935&usg=AOvVaw0-wlotjgl31E87ZKgKsu6F

My SOlution:-


