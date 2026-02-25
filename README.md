# leetcode_Analisis_de_algoritmos
Ejercicios semanales

Semana 1 :  ejercicio two number 

class Solution:

    """
    Docusing - FUERZA BRUTA
    complejidad de tiempo O(n2) se tiene dos bucles anidados
    se debe hacer nxn comparaciones
    """
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        n = len(nums)
        for i in range(n):
            for j in range(i + 1, n):
                if nums[i] + nums[j] == target:
                    return [i, j]
        return []
   
class Solution:     
    """
    Docusing - OPTIMIZACIÓN
    complejidad de tiempo O(n) se recorre una lista en 'num' una sola vez
    y uso de Hash Map que es una insercion en un diccionario 

    """
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        num_map = {}
        for i, num in enumerate(nums):
            complemento = target - num
            if complemento in num_map:
                return [num_map[complemento], i]
            num_map[num] = i
        return []

