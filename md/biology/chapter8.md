# Chapter 8: Trait Inheritance

# Introduction

### Genetics

**Traits:**

- Features which vary among organisms of a species
    - Such as color, height, etc.

**Heredity:**

- Process of traits transferring from parent to child

**Genetics:**

- Study of heredity

### Mendel

**Gregor Mendel:**

- Considered the father of modern genetics
- Studied heredity among organisms, most famously pea plants

### Alleles

**Gene:**

- Portion of DNA that contains instructions for a given feature

**Locus:**

- Plural: **Loci**
- Chromosomal location of a gene

**Allele:**

- Version of a gene; contains instructions for the specific trait manifestation of the gene’s feature
- Diploid organisms, such as humans, contain two alleles of each gene, one from each parent.
    - The two alleles are located at similar loci in their respective homologous chromosomes.

**Genotype:**

- An organism’s genetic makeup

**Phenotype:**

- An organism’s observable traits
    - Caused by the genotype

**Homozygous:**

- The two alleles for a given gene are identical

**Heterozygous:**

- The two alleles for a given gene are non-identical

---

# Mendelian Genetics

### Mendelian Genetics

**Overview:**

- In Mendelian genetics, non-identical alleles are classified as dominant and recessive. When an organism has heterozygous alleles, the dominant allele is expressed.
- A recessive allele is only expressed if the alleles are homozygous recessive.
- Although only the dominant allele is expressed, the organism contains the recessive allele. This recessive allele can be passed to the the organism’s offspring.
- Mendel deduced this from the observation that two parent organisms with a given phenotype can produce a child with a different phenotype. He explains that this happens when both parents have a dominant and recessive gene, and the child receives the recessive gene from both parents. In the parents, only the dominant gene is expressed, but in the child, the recessive gene is expressed.

### **Genotype Allele Notation**

**Notation:**

- The alleles of a genotype are notated with a pair of two letters, one for each allele.
- Both alleles use the same letter, generally the first letter of the phenotype of the gene’s dominant allele.
- A dominant gene is notated in uppercase, a recessive gene in lowercase.

Examples:

- `AA`
    - Two dominant `A` genes
    - Homozygous dominant
    - `A` is expressed
- `Aa`
    - Dominant `A`, recessive `a`
    - Heterozygous
    - `A` is expressed
- `aa`
    - Two recessive `a` genes
    - Homozygous recessive
    - `a` is expressed

### Mendelian Generations

In Mendel’s experiments, there are three main generations: P, F1 and F2

**P:**

- Purebred homozygous organisms.

**F1:**

- The first crossbred generation, bred from two Ps.

**F2:**

- The second crossbred generation, bred from two F1s.

### Monohybrid Cross

**Hybridization:**

- Mating organisms with the goal of producing offspring with a given phenotype

**Monohybrid:**

- Cross between two P organisms with non-identical phenotypes for a single trait

Mendel observed that, in a monohybrid cross:

- F1:
    - Although P parents had non-identical phenotypes, all F1 children had identical phenotypes, reflecting only one of the parents.
- F2:
    - Although only one P phenotypes were expressed in F1, both P phenotypes were expressed in F2.
    - The P phenotypes were expressed in F2 in a 3:1 ratio; 3 F2 with the same P phenotype as F1, 1 F2 with the P phenotype not in F1.

### Law of Segregation

**Law of Segregation:**

- Mendel’s First Law
- States that a parent’s two alleles are segregated into two gametes, and only one allele from each parent is passed to a child.

This explains the monohybrid cross:

- P:
    - Both Ps are homozygous, however, one is homozygous dominant `AA`, and one is homozygous recessive `aa`.
- F1:
    - Each F1 receives one allele from each parent - one `A` and one `a`.
    - This results in universal F1 `Aa` heterozygous genotypes.
    - As `A` is dominant and `a` is recessive, F1 universally expresses `A`.
- F2:
    - As all F1 are `Aa`, F1 gametes are 50% `A`, 50% `a`.
    - Between both F1 parents, there are four equally probably F2 genotypes:
        - `AA`:
            - `A` from both parents;
        - `Aa`:
            - `A` from parent #1 and `a` from parent #2;
        - `aA`:
            - `a` from parent #1 and `A` from parent #2; and
        - `aa`:
            - `a` from both parents.
    - Of these options, the first three express `A`, and the last expresses `a`, resulting in a 3:1 ratio.

### Punnett Square

**Punnett Square:**

- Method of visualizing child genotype possibilities by placing one parent’s genotype on top of a grid and the other’s on the side
- Example:
    - Punnett Square for parents with `Aa` and `aa`
        
        
        | | `A` | `a` |
        | --- | --- | --- |
        | `a` | `Aa`  | `aa`  |
        | `a`  | `Aa`  | `aa` |
    - 50% of children will express `A`; 50% will express `a`

### Dihybrid Cross

**Dihybrid Cross:**

- Cross between two P organisms with non-identical phenotypes for two separate traits

Mendel observed that, in a dihybrid cross:

- F1:
    - Although P parents had non-identical phenotypes for both traits, all F1 children had identical phenotypes for both traits.
- F2:
    - Although only one P phenotype for each trait was expressed in F1, all four possible P phenotype combinations were expressed in F2.
    - The P phenotypes were expressed in F2 in a 9:3:3:1 ratio; nine with phenotypes of both traits identical to F1; three with only one, three with only the other, and one with neither.

### Law of Independent Assortment

**Law of Independent Assortment:**

- Mendel’s Second Law
- States that alleles for different traits sort into gametes independently; the probability of inheriting one trait is independent of the probability of inheriting another
    - Example: For a parent with an `AaBb` genotype:
        - The `A` and `a` alleles will sort into gametes independent of the `B` and `b` assortment.
        - Each gamete has a 50% chance of receiving a `B` gamete and a 50% chance of receiving a `b` gamete, regardless of if they received an `A` or `a`
        - In total, there are four equally probable gamete genotypes:
            - `AB`
            - `Ab`
            - `aB`
            - `ab`

This explains the dihybrid cross:

- P:
    - Both Ps are homozygous for both traits, however, for each trait, one is homozygous dominant, and one is homozygous recessive.
- F1:
    - For both traits, each F1 receives a dominant allele from one parent, and a recessive allele from the other.
    - This results in universal F1 `AaBb` genotypes.
    - F1 universally expresses `AB`.
- F2:
    - As all F1 are `AaBb`, there are four gamete options for each parent.
    - This results in sixteen genotype options for F2:
    
    | | `AB` | `Ab` | `aB` | `ab` |
    | --- | --- | --- | --- | --- |
    | `AB` | `AABB`  | `AABb` | `AaBB` | `AaBb` |
    | `Ab` | `AABb` | `AAbb` | `AaBb` | `Aabb` |
    | `aB` | `AaBB` | `AaBb` | `aaBB` | `aaBb` |
    | `ab` | `AaBb` | `Aabb` | `aaBb` | `aabb` |
    - Of these options, nine express `AB`, three `Ab`, three `aB`, and one `ab`, resulting in a 9:3:3:1 ratio.

---

# Exceptions to Mendelian Genetics

### Polygenic, Multifactorial

**Polygenic:**

- Trait that is determined by numerous genes
    - Such as height and skin color
- Does not follow traditional Mendelian genetics

**Multifactorial:**

- Trait that is influenced by environmental factors as well as genetics
- Does not follow traditional Mendelian genetics

### Pleiotropic, Linked Genes

**Pleiotropic:**

- Gene that affects multiple traits
- Traits will not follow law of independent assortment

**Linked Genes:**

- Separate genes located on the same chromosome
- Genes are “linked” and do not follow the law of independent assortment

### Codominance, Incomplete Dominance

**Codominance:**

- Heterozygous genes that are simultaneously expressed
    - Example: Heterozygous color-determining genes resulting in spots of each color
    - Does not follow the Mendelian dominant-recessive model
    - Notation: `AB`

**Incomplete Dominance:**

- Heterozygous genes that are expressed in a blended form
    - Example: Heterozygous color-determining genes resulting in a universal blend of both colors
    - Does not follow the Mendelian dominant-recessive model
    - Notation: `Aa`

### X-Linked

**X-Linked Trait:**

- Select genes are present on the X sex chromosome but not on the Y sex chromosome. Since males only have one X chromosome, Mendelian genetics do not directly apply.

---
